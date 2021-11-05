<template>
     <div class="tag-container">


<input 
type="text" 
@keydown.enter="addTag"
@keydown.backspace="removeTag"
>
<div class="error" v-if="error">Bu etiket dah önceden eklenmis!!</div>
  </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>

</style>