<template>
  <div>
        <span class="tag" v-for="(tag,index) in tags" :key="tag">
        <span class="content">{{tag}}</span>
        <span class="close" @click="removeOneTag(index)">X</span>
    </span>
  </div>
</template>
<script>
export default {
    
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