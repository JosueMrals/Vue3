<script>
export default {
  data: () => ({
    contador: 0
  }),
  methods: {
    incrementar() {
      this.contador++;
    },
    decrementar() {
      this.contador--;
    },
    reset() {
      this.contador = 0;
    }
  }
};
</script>

<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="logo vue" width="250" height="250">
    <small>
      <h1>Hola mundo desde Vue.js 3</h1>
    </small>

    <hr />
    <h2>Contador: {{ contador }}</h2>
    <button @click="incrementar()">+1</button>
    <button @click="decrementar()">-1</button>
    <button @click="reset()">reset</button>
  </div>
</template>

<style scoped>
.container {
  text-align: center;
}

h1 { 
  font-weight: bolder;
}
h2 {
  font-size: 1.5rem;
}

button{
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 6px;
}

small{
  color: #666;
}

</style>
