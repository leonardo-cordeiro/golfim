<template>
  <div class="q-mb-md  text-center">
    <h1 class="text-h4 text-info text-raleway">
      Nossos
      <span style="text-decoration: underline">Trabalhos</span>
    </h1>
    <div class="carroussel q-py-md text-center" id="q-app">
      <div class="q-mx-auto">
        <q-carousel class="carousel q-mx-auto"
          animated
          v-model="slide"
          navigation
          infinite
          :autoplay="autoplay"
          arrows
          transition-prev="slide-right"
          transition-next="slide-left"
          @mouseenter="autoplay = false"
          @mouseleave="autoplay = true"
        >
          <q-carousel-slide class="slide" :name="1">
            <q-img height="100%" width="50rem" src="img/trabalho-1.webp?" fit="cover" class="framed-image"></q-img>
          </q-carousel-slide>
          <q-carousel-slide class="slide" :name="2">
            <q-img height="100%" width="50rem" src="img/trabalho-2.jpg?" fit="cover" class="framed-image"></q-img>
          </q-carousel-slide>
          <q-carousel-slide class="slide" :name="3">
            <q-img height="100%" width="50rem" src="img/trabalho-3.jpg?" fit="cover" class="framed-image"></q-img>
          </q-carousel-slide>
          <q-carousel-slide class="slide" :name="4">
            <q-img height="100%" width="50rem" src="img/trabalho-4.jpg?" fit="cover" class="framed-image"></q-img>
          </q-carousel-slide>
          <q-carousel-slide class="slide" :name="5">
            <q-img height="100%" width="50rem" src="img/trabalho-5.jpeg?" fit="cover" class="framed-image"></q-img>
          </q-carousel-slide>
          <q-carousel-slide class="slide" :name="6">
            <q-img height="100%" width="50rem" src="img/trabalho-6.jpeg?" fit="cover" class="framed-image"></q-img>
          </q-carousel-slide>
          <q-carousel-slide class="slide" :name="7">
            <q-img height="100%" width="50rem" src="img/trabalho-7.jpeg?" fit="cover" class="framed-image"></q-img>
          </q-carousel-slide>
        </q-carousel>
      </div>
    </div>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {
    return {
      slide: ref(1),
      autoplay: ref(true),
      fitModes: ['cover', 'fill', 'contain', 'none', 'scale-down']
    }
  }
}
</script>
<style scoped>

.slide {
  overflow: hidden;
  padding: 0;
}
.framed-image {
  max-width: 100%;
  border: 10px solid #075AA8; /* Adicione uma borda com uma cor mais atraente */
  box-sizing: border-box; /* Garante que a borda não aumente as dimensões da imagem */

}
@media (max-width: 700px) {
  .framed-image {
    border: 5px solid #075AA8;
     /* Ajuste a espessura da borda para 8px em telas menores que 700px */
  }
}

.carousel{
 max-width: 90%;
 width: 50rem;


}

</style>







