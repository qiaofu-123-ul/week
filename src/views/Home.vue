<template>
  <div>
      <div v-for="(item,index) in list" :key="index">
          <swiper :options="swiperOption">
           <swiper-slide><img :src="item.img" alt=""></swiper-slide>


          </swiper>
      </div>
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
            ],
            swiperOption:{
                  autoplay:true,
                  loop:true
            }

      }
  }
}
</script>
<style lang="scss" scoped>
 swiper{
  width: 100%;
  height: 200px;
 
  swiper-slide{
    width: 100%;
    height: 200px; 
    img{
      width: 100%;
      height: 200px;
      overflow: hidden;
    }
  }
 }


</style>
