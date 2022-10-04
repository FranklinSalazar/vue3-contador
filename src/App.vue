<script>
  export default {
    data: () => ({
      contador: 10,
    }),
    methods: {
      incrementar() {
        this.contador++;
      },
      disminuir() {
        this.contador--;
      },
      resetear() {
        this.contador = 10;
      },
    },
  }
</script>

<template>

  <div id="app" class="container">
    <fieldset>
      
      <img src="./assets/logo.svg" alt="Logo Vue" width="125" height="125">
    
      <small>
        <h1>My App en Vue.js 3</h1>
      </small>

    </fieldset>

    <hr>

    <fieldset>
    
      <h2>Contador: {{ contador }}</h2><br><br>

      <button @click="disminuir()">-1</button>
      <button @click="incrementar()">+1</button>
      <button @click="resetear()">Reset</button>

    </fieldset>

  </div>
  
</template>

<style scoped>
  .container {
    text-align: center;
  }

  h1 {
    font-weight: bolder;
  }

  small {
    color: #666;
  }

  h2{
    font-size: 2.5rem;
    font-weight: bolder;
  }

  button {
    cursor: pointer;
    font-size: 1.5rem;
    margin: 0px 6px;
    padding: 0.5rem 1rem;
    border-radius: 0.5rem;
    border: none;
    background-color: rgb(4, 0, 255);
    color: rgb(255, 255, 255);
  }

  fieldset{
    border: 1px solid rgba(247, 6, 6, 0.288);
    border-radius: 1.5rem;
    padding: 2rem;
    margin: 1rem 500px;
  }

  hr{
    border: 1px solid rgba(223, 68, 68, 0.24);
    border-radius: 0.5rem;
    margin: 1rem 450px;
  }

</style>