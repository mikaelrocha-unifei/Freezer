## Step 1: Passos iniciais para começar a programar

Para isso tive que pensar como poderia montar algo que se assemelhasse com um real _Freezer_, para tal tive que definir as opçoes para mostrar no LCD, entratanto as opções de ligar/desligar ventoinha e mostrar a temperatura seria algo muito simples, além disso a pessoa não teria paciência de ir no seu _Freezer_ e ficar toda hora verificando temperatura e ligando a ventoinha para manter nos padrões de fábrica, para isso implementei uma forma que ficasse automático, sem a necessidade do indivíduo ficar mexendo.

## Step 2: Adaptações da função `printf();`

Como estamos em um microcontrolador, tal função tão simples não tinha poder de imprimir algo no LCD, com isso tive que adaptar para que funcionasse e imprimisse _Strings_

![22](https://user-images.githubusercontent.com/75506742/101366799-286cf580-3884-11eb-9cb2-cb774c29d94c.png)

A função `printf1();` tem várias frases pré defininas para que eu escolhesse qual eu usaria, para selecionar foi necessário usar a variável "choice", dependendo de qual número ia vir resultaria em uma frase, como por exemplo nesta imagem, tal variável tinha seu valor igual a 2:

![33](https://user-images.githubusercontent.com/75506742/101366822-2e62d680-3884-11eb-9e1f-f64b0fc985a7.png)


## Step 3: O Funcionamento do menu

Para que ficasse mais formal e que o cliente tivesse noção do que os botões faziam, implementei um menu onde está dentro de um _for(;;)_ e um _switch(slot)_, a utilização de _cases_ ficaria mais fácil para direcionar as aplicações

![55](https://user-images.githubusercontent.com/75506742/101369249-d6799f00-3886-11eb-88eb-4f868e16f6c8.png)
![AAa](https://user-images.githubusercontent.com/75506742/101372002-2e65d500-388a-11eb-8251-053d99e4b1ca.png)

Como já supracitado, a função _printf1();_ foi constantemente utilizada para imprimir todas as opções, além disso foi acompanhada por funções que faziam a limpeza do LCD ou pular a linha para que coubesse as frases, como também atrasos para que o indivíduo pudesse ler com um tempo adequada para memorizar.

## Step 4: Varredura do teclado matricial

Como já citado, o _looping_ infito carrega com sigo mesmo um _switch_, onde o _slot = 1_ está a parte onde há a leitura de qual tecla está pressionada, além disso as opções são definidos por um _if();_, isso é, as teclas terão seus trabalhos programados aqui:

![77](https://user-images.githubusercontent.com/75506742/101370801-b814a300-3888-11eb-8e17-06d5cb01061f.png)

## Step 5: Funcionamento da ventoinha

A ventoinha tem uma função muito importante para que o sistema fique em temperaturas ideais, porém é necessário ter requisitos para que ela funcione de forma adequada, para isso tive que usar uma variável para verificar se duas opções estão ligadas ou desligadas, ou seja, a variável _vrf_(verficar se a mesma está on == 1 ou off == 0) e _vrfa_(verficar se o modo automatico esta ligada == 1)


