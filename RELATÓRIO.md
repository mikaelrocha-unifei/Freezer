## Step 1:Passos iniciais para começar a programar

Para isso tive que pensar como poderia montar algo que se assemelhasse com um real _Freezer_, para tal tive que definir as opçoes para mostrar no LCD, entratanto as opções de ligar/desligar ventoinha e mostrar a temperatura seria algo muito simples, além disso a pessoa não teria paciência de ir no seu _Freezer_ e ficar toda hora verificando temperatura e ligando a ventoinha para manter nos padrões de fábrica, para isso implementei uma forma que ficasse automático, sem a necessidade do indivíduo ficar mexendo.

## Step 2: Adaptações da função `printf();`

Como estamos em um microcontrolador, tal função tão simples não tinha poder de imprimir algo no LCD, com isso tive que adaptar para que funcionasse e imprimisse _Strings_

![22](https://user-images.githubusercontent.com/75506742/101366799-286cf580-3884-11eb-9cb2-cb774c29d94c.png)

A função `printf1();` tem várias frases pré defininas para que eu escolhesse qual eu usaria, para selecionar foi necessário usar a variável "choice", dependendo de qual número ia vir resultaria em uma frase, como por exemplo nesta imagem, tal variável tinha seu valor igual a 2:

![33](https://user-images.githubusercontent.com/75506742/101366822-2e62d680-3884-11eb-9e1f-f64b0fc985a7.png)


## Step 3: O Funcionamento do menu
