Basicamente o REST utiliza uma sintaxe de três pontinhos <strong>...</strong> normalmente para juntar itens/parâmetros em um array. Comumente utilizado em funções.
<br>
<p>
Já o operador Spread utiliza também a sintaxe de três pontinhos <strong>...</strong> mas normalmente para espalhar itens de um array, isso pode significar:
    ** Retirando todos os itens/parâmetros de um array ou de um objeto e adicionando-os em outro array ou adicionando-os a um objeto.
</p>
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



<b>Então basicamente o operador Rest vai pegar os itens e transformar em um array de itens</b>




<h3>Exemplo utilizando Spread em um Objeto</h3>
<br>
<pre>
let endereco = {'rua':"Av.Agamenon Magalhães", 'numero':220, 'cidade': Recife, 'estado':"Pernambuco", 'país':"Brazil"};

let pessoa = {'nome':"Kimbelly",...endereco}

console.log(pessoa);
</pre>
<br>
Teremos como retorno no console.log para o objeto pessoa
pessoa = 

{'nome':"Kimbelly",
'rua':"Av.Agamenon Magalhães", 
'numero':220, 'cidade': Recife, 
'estado':"Pernambuco", 
'país':"Brazil"};

<br>
<br>
<h3>Exemplo utilizando REST em uma função</h3>
<br>
<pre>
function soma(...numeros){
    let valorfinal = 0;
    for(let i=0; i<numeros.length ; i++){
        valorfinal+=i;
    }
    return valorfinal;
    
}
let paraprintar = soma(7,8,9,30);
console.log(paraprintar);
</pre>
<br>
retorno do console.log 54
<br>
<b> Então basicamente adicionamos os valores 7,8,9 e 30 em uma lista e passamos
para a função soma </b>
<br>
<br>
<pre>
function soma(a,maisnumeros){
    console.log(a);
    console.log(mmaisnumeros);
    let valorfinal = 0;
    for(let i=0; i<maisnumeros.length ; i++){
        valorfinal+=i;
    }
    valorfinal+=a;
    return valorfinal;
    
}
let paraprintar = soma(7,8,9,30);
console.log(paraprintar);
</pre>
<br>
retornos do console.log respectivamente
<br>7<br>
<br>[8,9,30]<br>
<br>54