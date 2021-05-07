<template>
    
      <div class="avt-summary-item1">
        <div class="avt-summary-color" >
            <img v-bind:src="image" alt="">
        </div>
        <div class="avt-summary-colors"  >

            <div class="avt-summary-colors-item" 
             v-for="image in images"
             :key="image"
             :class="[image.active ? 'avt-summary-colors-item--active' : '']"
             :id="image.id"
             @click="updateImage(image.img)"     
             >

                <img width="53" height="53" :src="image.thumb" alt="" @click="toggleActive(image.id)">
            </div>
        </div>
     
    </div>
 
</template>


<script>
export default {
  data() {
    return {
        image: require('@/assets/images/color_7024.jpg'),        
        images: [     
         { id: 1, img: require("@/assets/images/color_7024.jpg"), thumb:require("@/assets/images/color_7024_80_.jpg"), active: false },   
         { id: 2, img: require("@/assets/images/color_6005.jpg"), thumb:require("@/assets/images/color_6005_80_.jpg"), active: false },    
         { id: 3, img: require("@/assets/images/color_7016.jpg"), thumb:require("@/assets/images/color_7016_80_.jpg"), active: true },
         { id: 4, img: require("@/assets/images/color_8019.jpg"), thumb:require("@/assets/images/color_8019_80_.jpg"), active: false },        
         { id: 5, img: require("@/assets/images/color_8017.jpg"), thumb:require("@/assets/images/color_8017_80_.jpg"), active: false },        
         { id: 6, img: require("@/assets/images/color_3005.jpg"), thumb:require("@/assets/images/color_3005_80_.jpg"), active: false },
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
