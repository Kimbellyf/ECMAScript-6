Basicamente o REST utiliza uma sintaxe de três pontinhos <strong>...</strong> normalmente para juntar itens/parâmetros em um array. Comumente utilizado em funções.

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