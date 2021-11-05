<template>
 <div class="container">
<app-tags v-model="tags"></app-tags>

 </div>
</template>
<script>
import Tags from "./Component/Tags.vue"
export default {
 components:{
   appTags:Tags
 },
 data(){
   return{
     tags:"Vue,jquery"
   }
 }
}
</script>
<style >
body{
  font-family:sans-serif;
}

</style>
