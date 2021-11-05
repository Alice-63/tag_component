<template>
     <div class="tag-container">
         <Tag/>

<input 
type="text" 
@keydown.enter="addTag"
@keydown.backspace="removeTag"
>
<div class="error" v-if="error">Bu etiket dah önceden eklenmis!!</div>
  </div>
</template>
<script>
import Tag from "./Tag.vue"
export default {
    components:{
        Tag
    }
}
</script>
<style scoped>

.tag-container
{
  border: 1px solid #ccc;
  padding: 20px;
}
input{
  outline: none;
  height: 30px;
  width: 100px;
}

.error
{
  font-size: 12px;
  color: red;
  margin-top: 5px;
}
</style>