# Freezer

![AA](https://user-images.githubusercontent.com/75506742/101360186-15eebe00-387c-11eb-9ddb-e23dc7302d21.png)

### Como usar

Apos a inizialização do _freezer_ o próprio LCD dara as opções, tais como:

1. Verficar Temperatura - **Tecla 1**
4. Ligar Ventoinha - **Tecla 4**
7. Modo Automático da Ventoinha - **Tecla 7**
5. Rever Opções - **Tecla 5**

Como todo freezer ele tem suas especificações de temperatura, essas especificações ficam entre 1°C e 5°C para que tudo oque estiver dentro se mantenha gelado, por padrão a ventoinha se mantem desligada para manter em temperaturas mais "altas", isso é, próximas de 5°C, porém se o cliente sentir que não está gelado o suficiente a solução é ligar a ventoinha, consequentemente a temperatura ficará perto de 1°C. Entretanto, ficar mudando de forma manual não seja algo muito eficiente, para isso existe o **Modo Automático**, tal modo funciona em ligar e desligar a ventoinha em função da temperatura, ou seja, se x°C > 5°C irá soar um som avisando e ligará a ventoinha para abaixar a temperatura, como também ocorre quando x°C < 1°C, um som será ligado e a ventoinha será desligada.

### Como utilizar o código

O principal método é utilizar o [MPLAB X IDE](https://www.microchip.com/mplab/mplab-x-ide) com o compilador XC8, após isso é apenas baixar o arquivo compactado e importar tudo para o programa MPLab. Além disso, para poder executar e testar os códigos é necessário do [PICSimLab](https://github.com/lcgamboa/picsimlab), logo após baixar e iniciar vá na barra superior e clique em _Files_ -> _Load Hex_, o arquivo que será colocado está nesta pasta `PROJETO.X\dist\default\production\PROJETO.X.productions.hex`.

### Créditos

Projeto feito na Universidade Federal de Itajubá para a avaliação e supervisão dos professores [Rodrigo Almeida](https://github.com/rmaalmeida) e [Otavio Gomes](https://github.com/osmgomes)
