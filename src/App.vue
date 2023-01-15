<script>
export default{
  data:()=> ({
    contador : 0, 
  }) 
};
</script>



<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="logo vue" width="125" height="125" />
    <small> <h1>"hola mundo"</h1></small>
    <hr />
    <h2>contador {{contador}}</h2>
    <button v-on:click="contador++"> +1 </button>
    <button @click="contador --"> -1 </button>
    <button @click="contador = 0"> Reset </button>
  </div>
</template>

<style scoped>
.container {
  text-align: center
}
small{
  color: gray;
}
h2{
  font-size: 2.5rem;
}
button{
  cursor: pointer;
  font-size: 1.2rem;
  margin: 0px 6px;
}

</style>
