<template>
  <div class="block">
    <div class="slide"><img ref="slide" :src="require(`../assets/images/photos/${current}`)" alt=""></div>
    <div class="thumbs">
      <div class="thumb" v-for="(slide,i) in slides" :key="i" @click="showThisSlide(i)"><img :src="require(`../assets/images/photos/${slide}`)" alt=""></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Gallery",
  methods:{
    showThisSlide(index){
      this.current = this.slides[index]
    }
  },
  data() {
    return {
      current:'1-kulian.jpg',
      slides: [
        '1-kulian.jpg',
        '2-red-line-1.jpg',
        '2-red-line-3.jpg',
        '3-prorastanie-1.jpg',
        '4-cilynder-1.jpg',
        '4-cilynder-2.jpg',
        '4-cilynder-3.jpg',
        '4-cilynder-4.jpg',
        '4-cilynder-5.jpg',
        '4-cilynder-6.jpg',
        '5-struktura-gonobob-1.jpg',
        '5-struktura-gonobob-2.jpg',
        '5-struktura-gonobob-3.jpg',
        '5-struktura-gonobob-4.jpg',
        '6-sklad-1.jpg',
        '6-sklad-2.jpg',
        '6-sklad-3.jpg',
        '7-brus-1.jpg',
        '7-brus-3.jpg',
        '8-portal-1.jpg',
        '8-portal-2.jpg',
        '8-portal-3.jpg',
        '9-ogranichiteli.jpg',
        '10-kontrafore-1.jpg',
        '10-kontrafore-2.jpg',
        '11-nephotoelementy-2.jpg',
        '12-lisytsky.jpg',
        '13-kontraforce-1.jpg',
        '13-kontraforce-2.jpg',
        '14-makrame-1.jpg',
        '14-makrame-2.jpg',
        '14-makrame-3.jpg',
      ]
    }
  }
}
</script>

<style scoped>
.block {
  display: grid;
  grid-gap: 30px;
  grid-template-columns: 1fr;
  grid-template-rows: 1fr auto;
}

.slide {
  display: flex;
  object-fit: contain;
  justify-content: center;
  align-items: center;
  width: 100%;
  border-radius: var(--radius);
  overflow: hidden;
  max-height: 70vh;
}

.thumbs {
  overflow: auto;
  width: 100%;
  display: flex;
  flex-wrap: nowrap;
  border-radius: var(--radius);
}

.thumb {
  overflow: hidden;
  height: 152px;
  width: 213px;
  border-radius: var(--radius);
  margin-right: 30px;
  display: inline-block;
  white-space: nowrap;
  flex-shrink: 0;
  cursor: pointer;
}

.thumb img {
  height: 100%;
  display: flex;
}
@media (max-width: 420px) {

}
</style>