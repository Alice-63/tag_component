<template>
 <div class="container">
<app-tags v-model="tags" color="primary" ></app-tags>
{{tags}}
<hr>
<app-tags v-model="tags2" color="info" ></app-tags>
{{tags2}}
<hr>
<app-tags v-model="tags3" color="secondary" ></app-tags>
{{tags3}}
<hr>
<app-tags v-model="tags4" color="warning" ></app-tags>
{{tags4}}


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
     tags2:"tags2",
     tags3:"Tags3",
     tags4:"Tags4"
    
   }
 }
}
</script>
<style >
body{
  font-family:sans-serif;
}

</style>
