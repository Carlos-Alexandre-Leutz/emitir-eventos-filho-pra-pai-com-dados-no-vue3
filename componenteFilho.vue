<template>
  <div> 
    <button @click="minhaFuncao">adicionar evento </button>
  </div>
</template>
<script>
export default {
 methods: {
  minhaFuncao(){
    let data = "conteudo"; 
    this.$emit("nomeDoMEuEvento", data);
  }
 }
}
</script>
