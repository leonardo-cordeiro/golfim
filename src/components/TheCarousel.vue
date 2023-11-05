<template>
  <div class="q-pa-md text-center">
    <h1 class="text-h4 text-info text-raleway">
      Nossos
      <span style="text-decoration: underline">Trabalhos</span>
    </h1>
    <q-carousel
      v-model="slide"
      transition-prev="slide-right"
      transition-next="slide-left"
      swipeable
      animated
      control-color="info"
      navigation
      padding
      arrows
      height="300px"
    >
      <q-carousel-slide :name="1" class="column no-wrap">
        <div class="row fit justify-center items-center q-gutter-xs q-col-gutter no-wrap">
          <q-img class="rounded-borders col-3 full-height" src="img/trabalho-1.webp" />
          <q-img class="rounded-borders col-3 full-height" src="img/trabalho-2.webp" />
          <q-img class="rounded-borders col-3 full-height" src="img/trabalho-3.webp" />
        </div>
      </q-carousel-slide>
      <q-carousel-slide :name="2" class="column no-wrap">
        <div class="row fit justify-center items-center q-gutter-xs q-col-gutter no-wrap">
          <q-img class="rounded-borders col-3 full-height" src="img/img-servico2.webp" />
          <q-img class="rounded-borders col-3 full-height" src="img/img-servico3.webp" />
          <q-img class="rounded-borders col-3 full-height" src="public/img/trabalho-4.jpeg" />
        </div>
      </q-carousel-slide>
      <q-carousel-slide :name="3" class="column no-wrap">
        <div class="row fit justify-center items-center q-gutter-xs q-col-gutter no-wrap">
          <q-img class="rounded-borders col-3 full-height" src="public/img/trabalho-5.jpeg" />
          <q-img class="rounded-borders col-3 full-height" src="public/img/trabalho-6.jpeg" />
          <q-img class="rounded-borders col-3 full-height" src="public/img/trabalho-7.jpeg" />
        </div>
      </q-carousel-slide>
    </q-carousel>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {
    return {
      slide: ref(1)
    }
  }
}
</script>
