<template>
  <div class="wrap">
    <div class="image">
      <div class="row">
        <div class="col-md-7 col-xs-12 q-pr-md">
          <q-img src="img/logo_golfim.webp" alt="logo" width="10rem" />
          <h1 class="text-white text-bold text-raleway" style="font-size: 3rem">
            Reformas de
            <span style="text-decoration: underline">Piscinas</span>
          </h1>
          <h2 class="text-h5 text-white text-montserrat" >
            Consertos, Pinturas e Reformas de Piscinas com profissionais 100% qualificados!
          </h2>
          <h3 class="text-h6 text-white text-bold text-montserrat" >
            REPARO SUBMERSO: Trocamos os azulejos sem esvaziar a piscina.
          </h3>
        </div>
        <div class="col-md-5 col-xs-12 q-mt-lg text-center">
          <q-btn label="(21) 96483-3479" color="primary" icon="call" size="lg" href="tel:+5521964833479" rounded />
          <q-card class="card q-mt-sm" style="max-height: 100vh">
            <q-card-section class="text-center">
              <h4 class="text-h5 text-secondary text-bold">Solicite um Orçamento</h4>
            </q-card-section>

            <q-card-section class="q-px-xl">
              <q-form class="q-gutter-y-sm" @submit="submitForm">
                <q-input rounded v-model="name" outlined label="Nome Completo" :rules="[(val) => !!val || 'Insira seu Nome']" />
                <q-input type="textarea" rounded v-model="message" outlined label="Como podemos ajudar?" />
            
                <q-btn rounded label="Enviar" color="primary" class="full-width q-mb-xl" padding="14px" type="submit" />
              </q-form>
            </q-card-section>
          </q-card>
        </div>
        <a class="whatsapp-button" href="https://api.whatsapp.com/send?phone=5521964833479" target="_blank">
          <q-img src="/img/whatsapp.svg?" loading="eager" alt="WhatsApp" />
        </a>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
// import mySvgIcon from "public/whatsapp.svg"
import { useQuasar } from 'quasar'

const $q = useQuasar()
const name = ref('')
const message = ref('')

function submitForm() {
  const whatsappText = `Olá, sou ${name.value}. Gostaria de solicitar um orçamento para: ${message.value}`
  const whatsappLink = `https://api.whatsapp.com/send?phone=5521964833479&text=${encodeURIComponent(whatsappText)}`
  window.open(whatsappLink, '_blank')
  $q.notify({ message: 'Mensagem enviada com sucesso' })
}
</script>

<style lang="scss" scoped>
.wrap {
  height: 100%;
  width: 100%;

  .image {
    height: 100%;
    padding: 2rem;
    background-image: url('/img/background-header.webp?');
    background-repeat: no-repeat;
    background-size: cover;

      // Aumentar o tamanho do texto em telas pequenas
      @media screen and (max-width: 920px) {
      padding: 5rem;

      h2 {
        font-size: 2.5rem; // Altere o tamanho conforme necessário
      }

      h3 {
        font-size: 1.5rem; // Altere o tamanho conforme necessário
      }
    }

    @media screen and (max-width: 600px) {
      padding: 2rem;

      h2 {
        font-size: 2rem; // Altere o tamanho conforme necessário
      }

      h3 {
        font-size: 1.5rem; // Altere o tamanho conforme necessário
      }
    }
  }
}

.whatsapp-button {
  position: fixed;
  // background-image: url('public/img/whatsapp.svg');
  background-size: cover;
  width: 6rem;
  background-repeat: no-repeat;
  bottom: 50px;
  right: 50px;
  z-index: 999;
  font-size: 3rem;
  animation: whatsapp-bounce 1s infinite;

  @keyframes whatsapp-bounce {
    0%,
    20%,
    50%,
    80%,
    100% {
      transform: translateY(0);
    }
    60% {
      transform: translateY(10px);
    }
    80% {
      transform: translateY(5px);
    }
  }
}
// .phone-button {
//  display: flex;
//  align-items: center;
//   width: 50%;
// }

.card {
  height: 100%;
  width: 90%;
  border-radius: 1rem;
  margin-left: 1.5rem;
}

</style>