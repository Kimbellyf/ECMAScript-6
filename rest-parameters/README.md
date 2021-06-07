Basicamente o REST utiliza uma sintaxe de três pontinhos <strong>...</strong> para juntar itens.
<br>
<h3>Exemplo utilizando REST em uma lista</h3>
<br>
<pre>
let listaQualquer1 = ['oi', 'hello'];
let listaQualquer2 = ['opa','tudo bom?'];

let listasaudacoes = [...listaQualquer1,...listaQualquer2];
console.log(listasaudacoes);

</pre>
<br>
Teremos como retorno no console.log para a listasaudacoes
listasaudacoes = ['oi','hello','opa','tudo bom?'];
<br><br>
<h3>Exemplo utilizando REST em um Objeto</h3>
<br>
<pre>
let endereco = {'rua':"Av.Agamenon Magalhães", 'numero':220, 'cidade': Recife, 'estado':"Pernambuco", 'país':"Brazil"};

let pessoa = {'nome':"Kimbelly",...endereco}

console.log(pessoa);
</pre>
<br>
Teremos como retorno no console.log para a pessoa
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