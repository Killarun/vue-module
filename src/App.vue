<template>
  <div class='avt-main avt_vert_rythm_2'>
     <h2 class="avt-t05-h2">{{ title }}</h2>
    <h3 class="avt-t05-h3">{{ subtitle }}</h3>
    <div class="avt-t05-general-card">
    <div class="avt-t05-summary__header">
       
      <p class="avt-t05-summary__header-title">
        Металлочерепица Т05. Глянцевое покрытие
      </p>
      <p class="avt-t05-summary__header-description">
        Глянцевое покрытие – самое популярное на сегодня решение для кровли из
        металлочерепицы. Имеет гладкую поверхность, более высокую насыщенность
        цвета и блестит на солнце.
      </p>
   
    <div class="avt-summary">
      <Image />
      <Block />
    </div>
  </div>
  </div>
    </div>
</template>

<script>
import Image from './components/Image.vue'
import Block from './components/Block.vue'

export default {
  name: 'App',
  components: {
    Image,
    Block
  },
  data() {
    return {
      title: 'Металлочерепица Т05',
      subtitle: 'недорогая универсальная металлочерепица для кровли любой сложности',
    }
  }
}

</script>

<style>

</style>
