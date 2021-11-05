<template>
  
        <span class="tag">
        <span class="content">{{tag}}</span>
        <span class="close" @click="$emit('removeTagEvent',index)">X</span>
    </span>
  
</template>
<script>


export default {
    props:["tag","index"]
}
</script>
<style scoped>
.tag
{
  background-color: #fbbd08;
  padding: 10px;
  color: #000;
  cursor:default;
  font-size: 14px;
  margin-right: 5px;
}
.tag .close
{
  font-size: 12px;
  cursor: pointer;
  font-weight: bold;
}
</style>