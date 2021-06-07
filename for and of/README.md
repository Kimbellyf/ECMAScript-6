As instruções for/of JavaScript percorre os valores de objetos iteráveis.
<br>
for/of permite que você faça um loop em estruturas de dados que são iteráveis, como Arrays, Strings, Maps, NodeLists e muito mais.
<br>
O for/of loop tem a seguinte sintaxe:

<pre>
for (variable of iterable) {
  // code block to be executed
}
</pre>
variável - Para cada iteração, o valor da próxima propriedade é atribuído à variável. Variável pode ser declarada com const, let ou var.

iterável - Um objeto que possui propriedades iteráveis.

<h4>Loop em uma matriz exemplo com for:</h4>
Exemplo
<pre>
var cars = ["BMW", "Volvo", "Mini"];
var x;

for (x of cars) {
  document.write(x + "<br >");
}
</pre>
<br>


<h4>Loop em uma matriz exemplo com of:</h4>
Exemplo
<pre>
var cars = ["BMW", "Volvo", "Mini"];
var x;

for (x of cars) {
  document.write(x + "<br >");
}
</pre>
retorno do código acima:
<br>BMW<br>
Volvo<br>
Mini<br>
<br>

<h4>Exemplo sem of </h4>
<pre>
var cars = ["BMW", "Volvo", "Mini"];

for (let x=0; x< car.length; x++) {
  document.write(car[x] + "<br >");
}
</pre>
retorno do código acima:
<br>BMW<br>
Volvo<br>
Mini<br>
<br>
