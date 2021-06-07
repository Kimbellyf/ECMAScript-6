<p>Os operados de declaração de atributos antigamente em Javascript eram declarados somente como "Var" mas
a utilização dessa declaração para um atributo pode gerar algum tipo de confusão já que ela é uma variável global, não conseguindo muitas vezes separar o que foi feito em um escopo de função e de bloco (se caso tivesse o mesmo nome de atributo).</p>

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
<strong>Const</strong> é um operador de declaração utilizado para impedir que um atributo seja modificado em outras situações dentro do código.
</p>


<h5>Exemplos:</h5>
<br>
Exemplo usando declaração <strong>Let</strong>:
<br>

<pre>
let serie = 'The Boys'
{
    let serie = 'Csi'
    console.log('dentro do bloco: ' + serie)
}
console.log('fora do bloco' + serie)
</pre>

retorno dentro do bloco:
Csi

retorno fora do bloco:
The Boys


Exemplo usando <strong>Var</strong>:

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


retorno dentro do bloco pt 1 =
The Boys
retorno dentro do bloco pt 2 =
Csi
retorno fora do bloco =
The Boys


Exemplo usando <strong>Const</strong>:

<pre>
const serie = 'The Boys'
{
    console.log('dentro do bloco pt 1': ' + serie)
    const serie = 'Csi' // na vdd eu n posso declarar como const um atributo que ja foi declarado, isso vai gerar um erro
    serie = 'Csi' //esse também vai gerar erro porque eu não posso alterar uma const
    console.log('dentro do bloco pt 2': ' + serie)
}
 console.log('fora do bloco pt 2': ')
</pre>

retorno dentro do bloco pt 1 =
The Boys
retorno dentro do bloco pt 2 =
The Boys
retorno fora do bloco =
The Boys


