# ClientWS
Cliente js é uma simples API que visa facilitar a implementação do WebSockt JavaScript.

## Para utilizar
```js
<script src='wsApi.js'></script>
<script>
  ws.con("ws://localhost:8080");//abrindo a conexão
  ws.open(funcion(){alert('1º function')}); //Espera como parametro uma function de callback
  ws.open(funcion(){alert('2º function')}); //Open pode ser chamado quantas vezes for necessário
  ws.open(funcion(){alert('3º function')});
  ws.close(function(){alert('Conexão fechada')}); //Quando a conexão for fechada
  ws.message(funcion(e){alert(e.data)});    //quando recebe menssagem
  ws.send("Esta é uma menssagem para ser submetida");  //Enviando menssagem
</script>
```

