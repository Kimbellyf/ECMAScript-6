<p>Os operados de declaração de atributos antigamente em Javascript eram declarados somente como "Var" mas
a utilização dessa declaração para um atributo pode gerar algum tipo de confusão já que ela é uma variável global, não conseguindo muitas vezes separar o que foi feito em um escopo de função e de bloco (se caso tiver o mesmo nome de atributo).</p>

<img src="https://github.com/Kimbellyf/ECMAScript-6/blob/main/var-let-const/escopoglobalelocal.JPG">


</p> <b><i>Para isso então foram criados os operadores de declaração Let e Const </i></b></p>

<p>
<strong>Let</strong> respeita o escopo em que é declarado e o mesmo nome de atributo pode ser declarado em vários escopos diferentes. 
<ul>
    <li> Se ele for declarado em escopo global o atributo vai ter o valor das modificações feitas no atributo dentro do escopo global. </li>
    <li>Se ele for declarado em escopo de função ele vai ter o valor das modificações feitas no atributo dentro do escopo de função</li>
    <li>Se ele for declarado em escopo de bloco ele vai ter o valor das modificações feitas no atributo dentro do escopo de bloco
    </li>
</ul>

<p>
<strong>Const</strong> é um operador de declaração utilizado para impedir que um atributo seja modificado em outras situações dentro do código. Também respeita o escopo em que foi declarado.
</p>


<h3>Exemplos:</h3>
<br>
<h5>Exemplo usando declaração <strong>Let</strong>:</h5>
<br>

<pre>
let serie = 'The Boys'
{
    let serie = 'Csi'
    console.log('dentro do bloco: ' + serie)
}
<br><br>
console.log('fora do bloco' + serie)
</pre>
<br>
retorno dentro do bloco:
Csi
<br>
retorno fora do bloco:
The Boys
<br><br>

<h5>Exemplo usando <strong>Var</strong>:</h5>

<pre>
var serie = 'The Boys'
{
    console.log('dentro do bloco pt 1': ' + serie)
    var serie = 'Csi' // na vdd eu n posso declarar como var um atributo que ja foi declarado, isso vai gerar um erro, só podendo fazer portanto o de baixo
    serie = 'Csi'
    console.log('dentro do bloco pt 2': ' + serie)
}
 console.log('fora do bloco pt 2': ')
</pre>

<br><br>
retorno dentro do bloco pt 1 =
The Boys
<br>
retorno dentro do bloco pt 2 =
Csi
<br>
retorno fora do bloco =
Csi
<br>
<br>
<h5>Exemplo usando <strong>Const</strong>:</h5>

<pre>
const serie = 'The Boys'
{
    console.log('dentro do bloco pt 1': ' + serie)
    const serie = 'Csi' 
    serie = 'Dark' //esse vai gerar erro porque eu não posso alterar uma const. Ela ja foi declarada dentro do escopo de bloco como 'Csi'
    console.log('dentro do bloco pt 2': ' + serie)
}
 console.log('fora do bloco pt 1': ')
 const serie = 'Stranger Things'; //vai dar erro pois a variável ja foi declarada no escopo global
 console.log('fora do bloco pt 2': ')
 serie = 'Stranger Things'; //vai dar erro pois a variável ja foi definida como 'The Boys' no escopo global e como const não pode mudar...
</pre>

<br><br>
retorno dentro do bloco pt 1 =
error.... (ela não foi inicializada então dará erro)
<br>
retorno dentro do bloco pt 2 =
Csi
<br>
retorno fora do bloco pt 1 =
The Boys
<br>
retorno fora do bloco pt 2 =
The Boys
<br>

