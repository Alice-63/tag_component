<template>
 
</template>
<script>
export default {
  data(){
    return{
      tags:["Vue","jquery"],
      error:false,
    }
  },
  methods:{
    addTag(event){
      let text=event.target;
      let matchedTag=false
      if(text.value.length>0)
      {
         this.tags.forEach(tag=>{
           if(tag.toLowerCase()===text.value.toLowerCase())
           {
            matchedTag=true;
           }
      
         })

         if(!matchedTag)
         {
           this.tags.push(text.value);
           text.value=""
         }
         else{
           this.error=true;
           setTimeout(()=>{
             this.error=false;
           },2000)
         }


      }

      
     
    },
    removeTag(e){

      if(e.target.value==0){
        
      this.tags.splice(this.tags.length-1,1)
      }
    },
    removeOneTag(index){
      this.tags.splice(index,1)
    }
  }
}
</script>
<style >
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

.error
{
  font-size: 12px;
  color: red;
  margin-top: 5px;
}
</style>
