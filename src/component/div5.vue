<template>
  <div  v-bind:style='{"background-color" : (flag ? "green" : "violet" )}' @click="chng()"> 
     <h4>ID-5</h4> 

   <p><b>Color:{{stylobj.backgroundColor}}</b></p>
  </div>
</template>

<script>
export default {
   components:{

  },
   props:['flag'],

  data() {
    return {
      //  flag:true,
        stylobj:{
    backgroundColor:'green' 
  }

    }
  },
  methods: {
     chng:function(event){
 if(this.flag = !this.flag){
      this.stylobj.backgroundColor = "green";
    }
    else{
      this.stylobj.backgroundColor = "Violet";
    }
  
 
}
}
  }

</script>

<style scoped>
.five {
 /* display: inline-block;  */
margin-left: 0 auto;
padding: 10px;
border-radius: 30px;
}
.green{
  background:green;
}
.violet{
  background: violet;
}
</style>
