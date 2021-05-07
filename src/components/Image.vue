<template>
    
      <div class="avt-summary-item1">
        <div class="avt-summary-color" >
            <img v-bind:src="image" alt="">
        </div>
        <div class="avt-summary-colors"  >

            <div class="avt-summary-colors-item" 
             v-for="(image, index) in images"
             :key="image"
             
             
             :class="[activeIndex === index ? 'avt-summary-colors-item--active' : '']"
             @click="updateImage(image.img)"     
             >

                <img width="53" height="53" :src="image.thumb" alt="" @click="onClickBlock(index)">
            </div>
        </div>
     
    </div>
 
</template>


<script>
export default {
  data() {
    return {
        image: require('@/assets/images/color_7024.jpg'),  
        activeIndex: 2,     
        images: [     
         { img: require("@/assets/images/color_7024.jpg"), thumb:require("@/assets/images/color_7024_80_.jpg") },   
         { img: require("@/assets/images/color_6005.jpg"), thumb:require("@/assets/images/color_6005_80_.jpg") },    
         { img: require("@/assets/images/color_7016.jpg"), thumb:require("@/assets/images/color_7016_80_.jpg")},
         { img: require("@/assets/images/color_8019.jpg"), thumb:require("@/assets/images/color_8019_80_.jpg") },        
         { img: require("@/assets/images/color_8017.jpg"), thumb:require("@/assets/images/color_8017_80_.jpg")},        
         { img: require("@/assets/images/color_3005.jpg"), thumb:require("@/assets/images/color_3005_80_.jpg")},
      ]
    };
  },
  
 

  methods: {
      updateImage(imageThumb){
          this.image = imageThumb
      },
  
   toggleActive(id){
        this.images = this.images.map((image) => image.id === id ? {...image, active: !image.active} : image)
        // console.log(id)
      },
      onClickBlock(index){
      if (this.activeIndex === index) {
      	this.activeIndex = 2;
      } else {
	    	this.activeIndex = index;
      }
    }
  }

  //   onDelite(id){
  //       this.images = this.images.filter((image) =>image.id !==id)
  // },
  



}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>



</style>
