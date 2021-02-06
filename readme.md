# Rocketseat - Guia Estelar de CSS

Neste curso iremos aprender o básico de CSS com _**Mayk Brito**_ da Rocketseat

Temos o site [W3 Schools](https://www.w3schools.com/) que fala sobre tudo detalhadamente do CSS

>Nenhuma aplicação web vive sem CSS, sem um visual e nesse guia vamos entrar de cabeça no mundo das estilizações da web.

## Aula 01 - Abertura
Iremos ver que utilização do CSS para personalizar os sites e aplicativos é a melhor opção pois eles ficaram incríveis, para isso teremos que aprender sobre seu fundamento, funcionamento, cascata, especificidade, box mode, seletores e muito mais

## Aula 02 - Conhecendo o CSS
CSS é a abreviação de Cascading Style Sheet que possui o significo de folha de estilo em cascata
Ele é um código para criar estilos no HTML, CSS é a beleza e o HTML é uma estrutura

Ela é uma linguagem de style sheet pois possui sínteses

Temos o site [Code Pen](https://codepen.io/pen/) que permite a utilização fácil dentre o HTML, CSS e JavaScript, assim você consegue unir os comandos dos três e ir visualizando o que acontece instantaneamente

## Aula 03 - Comentários
Como nas demais linguagens o CSS também contem o recurso de comentários, devemos usar pois ele ajuda deixando dicas para os outros entenderem com facilidade oque os comando estão realizando ou até nos mesmo depois de muito tempo de criar eles
````
/* MUDA UM POUCO COMO ATIVAR */
````

## Aula 04 - Anatomia
Para criar uma estilização vamos precisar de quatro itens
* Selector: É a tag do HTML que vai receber a estilização
  * h1
* Declaration: É o conjunto de tudo dentro das chaves
  * {...}
* Properties: É o código que vai realizar certa estilização
  * color
* Property value: É o valor que o properties vai receber
  * blue
````
h1 {
  color: blue;
  font-size: 60px;
  background: gray;
}
````
## Aula 05 - Seletores
Os seletores ou tag servem para conectar o elemento HTML com o CSS
````
Seletor global: *
Elemento ou tipo seletor: h1, h1, p, div e outros
ID seletor: #valorID
Classe seletor: .nomeClasse
````

Futuramente iremos ver sobre os attribute selector, Pseudo-class e outros

## Aula 06 - Box model
O CSS trabalha com o conceito de box model onde ele é o espaço onde o conteúdo se encontra, não existe um conteúdo sem uma box model

## Aula 07 - Origem do CSS
Existe quatro formas de adicionar o CSS em um arquivo HTML, os dois primeiro métodos não são recomendados pois eles vão aumentar muito as linhas de código no seu arquivo misturando as estilizações com as linhas de comandos

O método é composto na utilização de um atributo de uma tag como abaixo
````
<h5 style="font-size: 50px">Estilização inline 1 props</h5>
<h6 style="font-size: 45px; color: darkred">Estilização inline 2 props</h6>
````

No método tag usamos o próprio style no cabeçalho
````
<style>
  h4 {
    color: dimgrey;
    font-size: 30px;
    margin: 20px;
  }
</style>
````

Usando o link no cabeçalho é o melhor método de estilizar diretamente o HTML
````
<link rel="stylesheet" href="./style.css">
````

E por último as importações onde elas geram um pouco de atraso nos de sites terceiros
````
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script&display=swap');
````

## Aula 08 - A Cascata
É a regra de aplicar dos comandos de estilização, existe 3 fatores que devem ser obedecidos para poder executar uma boa estilização
* Origem do estilo
* Especificidade
* Importância

Na aula anterior vimos os tipos de vínculos de estilização do CSS com o HTML, onde uma consegue sobrepor a outra sendo que o **atributo style** é o mais forte de todos, depois temos a **tag style** e por último a tag link que é a importação mais elas possui o mesmo poder de aplicação, tudo isso é a origem do estilo

A cascata também possui a regra onde o último comando de estilização do mesmo tipo é a que vai ser aplicada sobrepondo todos anteriores
