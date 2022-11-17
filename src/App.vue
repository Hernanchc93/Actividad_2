<template>
  <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Problema 6</title>
</head>
<body>
    <h1>Area de un Circulo</h1>
    <p>Indique el radio del circulo para encontrar su area.</p>
    <p><input type="number" id="numero">
    <button type="button" id="btnValidar" onclick="areaCirculo()">Validar</button></p>
    <h2>Respuesta</h2>
    <p id="respuesta"></p>
</body>
</template>

<script>
import HelloWorld from './components/actividad2.vue'

/*export default {
  name: 'App',
  components: {
    HelloWorld
  }
}*/
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
