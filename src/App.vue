<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <br />
  <input type="number" v-model="radio" />
  <button @click="areaCirculo">Calcular area</button>
  <p>El área es <strong>{{ resultado }}</strong></p>

  <input type="number" v-model="num1" />
  <input type="number" v-model="num2" />
  <button @click="suma">Calcular Suma</button>
  <p>El resultado de la suma es <strong style="color: red">{{ resultadosuma }}</strong></p>


  <actividad2 msg="Area del circulo" />

</template>

<script>
import actividad2 from './components/actividad2.vue'

export default {
  name: 'App',
  data() {
    return {
      radio: 1,
      resultado: 0,
      num1: 0,
      num2: 0,
      resultadosuma: 0,
    }
  },
  components: {
    actividad2
  },
  methods: {
    areaCirculo() {
      this.resultado = ((Math.PI) * (Math.pow(this.radio, 2)))
    },
    suma() {
      if (this.num1 > 0 && this.num2 > 0) {
        this.resultadosuma = this.num1 + this.num2
      }
      else {
        alert("Digite numero mayor a 0")
      }

    }
  }
}
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
