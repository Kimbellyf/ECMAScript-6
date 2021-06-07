  Antes do ECMAScript6 o paradigma/padrão de Orientação a Objeto no JavaScript era mais confuso então o ECMAScript6 foi o responsável
  por deixar mais simples.


  <h4>Exemplo de como escrever um código JavaScript de maneira procedural </h4>
  <pre>
  let a = 20
  let b = 40
  let operador = '';
  
    function calcular(a,b, operador){
      if(operador=='*'){
        return a*b;
      }
      ...
    }
    let retornocalc = calcular(a,b,'*');
    console.log(retornocalc)
  
  </pre>
  
  <br>
  <h4>Exemplo de como escrever um código JavaScript de maneira Orientada a Objeto </h4>
  <pre>
  class Calculadora{
    constructor(){
      this.a = 20
      this.b = 40
    }

    function calcular(a,b, operador){
      if(operador=='*'){
        return a*b;
      }
      ...
    }
    let calcularAqui = new Calculadora(30,40,'*');
    console.log(calcularAqui);
  </pre>
  
