<template>
  <div id="app">
    <nav>
    <router-link to="/" tag="span">首页</router-link>
    <router-link to="/about" tag="span">医疗</router-link>
    </nav>
    
    <router-view/>
  </div>
</template>
<script>
export default {
  data(){
      return{
            list:[
              {
                img:"https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=1548509200,3423898172&fm=26&gp=0.jpg",
                title:"中国"
              },
                {
                img:"https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=3295174058,1884872095&fm=26&gp=0.jpg",
                title:"美国"
              },
              {
                img:"https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=2083352004,97320740&fm=26&gp=0.jpg",
                title:"德国"
              }
            ] 
      }
  }
}
</script>
<style lang="scss">
*{
  margin:0;
  padding:0; 
} 
html,body{
  width:100%;
  height:100%; 
}
#app{
  width:100%;
  height:100%;
  overflow: hidden;
  display:flex;
  flex-direction:column;
  nav{
     width: 100%;
     height: 50px;
     display: flex; 
     span{
      flex:1;
      text-align:center;
      line-height:50px;
     justify-content: space-between;
     }
  }
}
</style>
