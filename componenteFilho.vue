<template>
  <div> 
    <button @click="minhaFuncao">adicionar evento </button>
  </div>
</template>
<script>
export default {
//ex do msm evento  no setup
 emits: ["nomeDoMEuEvento"],
setup(context) {
 context.emit("nomeDoMEuEvento");
 retun{}
}
 methods: {
  minhaFuncao(){
    let data = "conteudo"; 
    this.$emit("nomeDoMEuEvento", data);
  }
 }
}
</script>
