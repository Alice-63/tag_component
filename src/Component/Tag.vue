<template>
  
        <span class="tag" :class="selectedTheme">
        <span class="content">{{tag}}</span>
        <span class="close" @click="$emit('removeTagEvent',index)">X</span>
    </span>
  
</template>
<script>


export default {
    props:["tag","index","tagColor"],
    data(){
      return {
        selectedTheme:null
      }
    },
    created(){
      this.selectedTheme=tagColor
    }
}
</script>
<style scoped>
.primary{
  color: #004085;
  background-color: #cce5ff;
  border-color: #b8daff;
}



.tag
{

  padding: 10px;

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