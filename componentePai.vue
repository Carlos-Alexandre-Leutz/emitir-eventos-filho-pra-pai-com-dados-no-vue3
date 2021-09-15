<template>
  <div>
    <Filho v-on:nomeDoMEuEvento="recebeEvento">
    </Filho>
  </div>
</template>
<script>

</script>
import Filho from "./componenteFilho";
export default {
    components: {
    Filho
    
    },
    setup() {
    const recebeEvento = (e) =>{
       console.log("data do componente filho" , e)
    
    }
    return {recebeEvento}
    
  }
