<template>
  <div class="wrap">
    <div class="image">
      <div class="justify-between row">
        <div class="col-md-7 col-xs-12 q-pr-md">
          <q-img src="img/logo_golfim.webp" alt="logo" width="10rem" />
          <h1 class="text-white text-bold text-raleway" style="font-size: 50px">
            Reformas de <span style="text-decoration: underline">Piscinas</span>
          </h1>
          <h2 class="text-h5 text-white text-montserrat" style="font-size: 22px">
            Consertos, Pinturas e Reformas de Piscinas com profissionais 100% qualificados!
          </h2>
          <h3 class="text-h6 text-white text-bold text-montserrat" style="font-size: 15px">
            REPARO SUBMERSO: Trocamos os azulejos sem esvaziar a piscina.
          </h3>
        </div>
        <div class="col-md-5 col-xs-12 text-center">
          <q-btn
            label="(21) 96483-3479"
            color="primary"
            icon="call"
            size="lg"
            href="tel:+5521964833479"
            rounded
          />
          <q-card class="q-mt-xl">
            <q-card-section class="text-center">
              <h4 class="text-h5 text-secondary text-bold">Solicite um Orçamento</h4>
            </q-card-section>

            <q-card-section class="q-px-xl">
              <q-form class="q-gutter-y-sm" @submit="notify">
                <q-input
                  rounded
                  v-model="name"
                  outlined
                  label="Nome Completo"
                  :rules="[(val) => !!val || 'Insira seu Nome']"
                />
                <q-input
                  rounded
                  v-model="whatsapp"
                  outlined
                  label="Whatsapp"
                  :rules="[(val) => !!val || 'Insira Seu Whatsapp']"
                  mask="(##) #####-####"
                />
                <q-btn
                  rounded
                  label="Enviar"
                  color="primary"
                  class="full-width q-mb-xl"
                  padding="14px"
                  type="submit"
                />
              </q-form>
            </q-card-section>
          </q-card>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { useQuasar } from 'quasar'

const $q = useQuasar()
const name = ref('')
const whatsapp = ref('')

function notify() {
  $q.notify({ message: 'mensagem enviada com sucesso' })
}
</script>

<style lang="scss" scoped>
.wrap {
  height: 100vh;
  width: 100vw;

  .image {
    height: 80%;
    width: 100%;
    padding: 12rem;
    background-image: url('img/background-header.webp');
    background-repeat: no-repeat;
    background-size: cover;
    @media screen and (max-width: 920px) {
      padding: 10rem;
    }
    @media screen and (max-width: 600px) {
      padding: 5rem;
    }
  }
}
</style>
