Os parâmetros default são paramêtros pré definidos que colocamos nas nossas funções para que caso não seja recebido o parâmetro na chamada da respectiva função
o parâmetro não fique como <b>undefined</b> e sim com um valor padrão.

<br>
<h3>Exemplos</h3>
<h5>Sem usar o parâmetro default:</h5>
<br>
<pre>
function soma(valorUm, valorDois){
  return valorUm + valorDois;
}
console.log(soma(3))
</pre>
<br>
no retorno do console vai vir soma = undefined

<br><br>
<h5>Utilizando o parâmetro default:</h5>
<br>
<pre>
function soma(valorUm, valorDois=0){
  return valorUm + valorDois;
}
console.log(soma(3))
</pre>
<br>
no retorno do console vai vir soma = 3
