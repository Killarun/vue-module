<template>
    
      <div class="avt-summary-item1">
        <div class="avt-summary-color" v-for="image in images" :key="image.id">
          <img
            :alt="image.alt"
            :src="image.img"
            :id="image.id"
            v-show="image.makeVisible"
          />
          <div class="avt-summary-color-tag">
            <div
              class="avt-summary-color-tag-code"
              v-show="image.makeVisible"
            >
               {{ image.dataColor}}
            </div>
            <div
              class="avt-summary-color-tag-name"
              v-show="image.makeVisible"
            >
              {{image.dataColorName}}
            </div>
          </div>
        </div>
        <div class="avt-summary-colors">
          <div
            
            v-for="(img, idx) in thumbimg" 
            :key="img"
            :class="img.class"
            @click="change(idx)"
            
          >
            <img 
            width="53" 
            height="53" 
            class="" 
            :id='idx+1' alt="" 
            :src="img.thumbimg"
            @click="remove()" 
            />
          </div>
        </div>
     
    </div>
 
</template>


<script>
export default {
  data() {
    return {
      images: [
        {
          id: 1,
          dataColor: "Цвет RAL 7024",
          dataColorName: "серый графит",
          alt: "серый графит",
          img: require("@/assets/images/color_7024.jpg"),          
          makeVisible: true
          
        },
         {
          id: 2,
          dataColor: "Цвет RAL 6005",
          dataColorName: "зеленый мох",
          alt: "серый графит",
          img: require("@/assets/images/color_6005.jpg"),      
          
          
        },
         {
          id: 3,
          dataColor: "Цвет RAL 6005",
          dataColorName: "серый графит",
          alt: "серый графит",
          img: require("@/assets/images/color_7016.jpg"),        
         
          
        },
         {
          id: 4,
          dataColor: "Цвет RAL 6005",
          dataColorName: "серый графит",
          alt: "серый графит",
          img: require("@/assets/images/color_7016.jpg"),      
          
          
        }
        ,
         {
          id: 5,
          dataColor: "Цвет RAL 6005",
          dataColorName: "серый графит",
          alt: "серый графит",
          img: require("@/assets/images/color_8017.jpg"),  
          
          
        }
        ,
         {
          id: 6,
          dataColor: "Цвет RAL 6005",
          dataColorName: "серый графит",
          alt: "серый графит",
          img: require("@/assets/images/color_3005.jpg"),         
          
          
        }
      ],
      thumbimg: [
          {   
              thumbimg:require("@/assets/images/color_7024_80_.jpg"),
              class: 'avt-summary-colors-item avt-summary-colors-item--active'
          },
          {   
              thumbimg:require("@/assets/images/color_3005_80_.jpg"),
              class: 'avt-summary-colors-item'
          },
          {   
              thumbimg:require("@/assets/images/color_3005_80_.jpg"),
              class: 'avt-summary-colors-item'
          },
          {   
              thumbimg:require("@/assets/images/color_3005_80_.jpg"),
              class: 'avt-summary-colors-item'
          },
          {   
              thumbimg:require("@/assets/images/color_3005_80_.jpg"),
              class: 'avt-summary-colors-item'
          },
          {   
              thumbimg:require("@/assets/images/color_3005_80_.jpg"),
              class: 'avt-summary-colors-item'
          }
      ]
    };
  },
  methods: {
    change: function(idx) {
      console.log(idx)
     
    },
    remove: function(){
        
    }
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>



</style>
