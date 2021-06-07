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

