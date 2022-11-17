<template>

</template>

<script>
/**
 * Calcule el área de un círculo (se debe pedir al usuario los datos para el cálculo). Imprima el resultado.
 */

 'use strict';

 const areaCirculo=()=>{
    let numero = document.getElementById("numero").value;
    let pi = Math.PI;
    console.log(numero);
    numero = parseFloat(numero);
    let area = ((pi)*(Math.pow(numero,2)));
    document.getElementById("respuesta").innerHTML = `El area del circulo es: ${area.toFixed(2)}`
 }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
