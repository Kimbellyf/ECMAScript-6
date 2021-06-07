
<p>
O operador Spread utiliza também a sintaxe de três pontinhos <strong>...</strong> mas normalmente para espalhar itens de uma string ou de um array, isso pode significar:
    ** Retirando todos os itens/parâmetros de um array ou de um objeto e adicionando-os em outro array ou adicionando-os a um objeto.
</p>
<h3>Exemplo utilizando Spread em uma String</h3>
<br>
<pre>
let palavra = 'vaca';
console.log(palavra);

</pre>
<br>Teremos como retorno no console.log uma string ' v a c a ';
<br><br>
<h3>Exemplo utilizando Spread em uma lista</h3>
<br>
<pre>
let listaQualquer1 = ['oi', 'hello'];
let listaQualquer2 = ['opa','tudo bom?'];

let listasaudacoes = [...listaQualquer1,...listaQualquer2];
console.log(listasaudacoes);

</pre>
<br>
Teremos como retorno no console.log para a listasaudacoes uma lista com os itens
tanto da listaQualquer1 quanto da listaQualquer2 resultando em:
listasaudacoes = ['oi','hello','opa','tudo bom?'];
<br><br>
<b>Então basicamente o operador Spread vai pegar os itens dentro do array e espalhar eles em outro array de itens</b>



