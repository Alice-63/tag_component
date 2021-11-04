<template>
  <div class="tag-container">
<span class="tag" v-for="tag in tags" :key="tag">
  <span class="content">{{tag}}</span>
  <span class="close">X</span>
</span>

<input type="text" @keydown.enter="tags.push($event.target.value)">
  </div>
</template>
<script>
export default {
  data(){
    return{
      tags:["Vue","jquery"],
    }
  }
}
</script>
<style scoped>
body{
  font-family:sans-serif;
}
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
