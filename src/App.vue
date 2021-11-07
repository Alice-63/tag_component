<template>
 <div class="container">
<app-tags v-model="tags" class="primary" ></app-tags>
{{tags}}


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
     tags:"Vue,jquery,Ali",
    
   }
 }
}
</script>
<style >
body{
  font-family:sans-serif;
}

</style>
