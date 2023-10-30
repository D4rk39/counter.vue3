

<script>

export default 
{
  data:() => ({
    contador : 10
  }),
  methods:{
    incrementar(){this.contador++;},
    disminuir(){this.contador--;},
    reset(){ this.contador = 0;},
  }
};


</script>
<template>
<div class="container">

  <img src ="./assets/logo.svg" alt="logo vue" width="125" height="125" />
  <small><h1>Prueba laravel</h1></small>
  <hr/>

  <h2> contador {{contador}}</h2>
  <button @:click="incrementar()">+1</button>
  <button @:click="disminuir()">-1</button>
  <button @:click="reset()">reset</button>
</div>
</template>

<style scoped>

.container{

text-align : center;
background-color: gray;
}

h1{font-weight: bolder; }

h2{font-size: 2.5rem; }

button{
  cursor: pointer;
  font-size: 2.5rem;
  margin: 0px 6px;
} 

</style>