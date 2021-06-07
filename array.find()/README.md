<br>
O find() método retorna o primeiro elemento em uma matriz que passa em um teste (fornecido como uma função).
<br>
O método find () executa a função uma vez para cada elemento presente na matriz:
<br>
Se encontrar um elemento da matriz onde a função retorna um valor verdadeiro , find () retorna esse elemento da matriz (e não verifica os valores restantes)
<br>
Caso contrário, retorna undefined
<br><br>
Nota: find () não executa a função para elementos do array sem valores.
<br>
Nota: find () não altera a matriz original.
<br>
fonte: 
<a href="https://www.w3schools.com/jsref/jsref_find.asp">Clique aqui</a>

<br>
Obtenha o primeiro elemento na matriz que tem um valor de 18 ou mais:

<pre>

var ages = [3, 10, 18, 20];

function checkAdult(age) {
  return age >= 18;
}

function myFunction() {
  document.getElementById("demo").innerHTML = ages.find(checkAdult);
}
</pre>