<template>
 <div class="container">
<app-tags v-model="tags"  ></app-tags>
{{tags}}
<hr>
<app-tags v-model="tags2"  ></app-tags>
{{tags2}}
<hr>
<app-tags v-model="tags3"  ></app-tags>
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
    tags2:"Vue,jquery,Ali",
    tags3:"Vue,jquery,Ali"
   }
 }
}
</script>
<style >
body{
  font-family:sans-serif;
}

</style>
