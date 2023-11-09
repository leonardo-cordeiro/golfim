<template>
  <div class="flex justify-evenly items-center text-montserrat q-pb-xl display q-pt-xl q-mt-xl q-mr-xl q-ml-xl">
    <div class="icon">
      <q-img class="img" src="img/icone-1.png" fit="contain" />
      <p>30 anos no mercado</p>
    </div>
    <div class="icon">
      <q-img class="img" src="img/icone-2.png" fit="contain" />
      <p>Técnicos com treinamento e experiência</p>
    </div>
    <div class="icon">
      <q-img class="img" src="img/icone-3.png" fit="contain" />
      <p>Serviços Personalizados</p>
    </div>
    <div class="icon">
      <q-img class="img" src="img/icone-4.png" fit="contain" />
      <p>Trabalhos Submersos</p>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.icon {
  width: 10rem;
  max-width: 50%;
  text-align: center;
  align-content: center;
  color: $accent;
  font-weight: bold;

  .img {
    padding: 0 1rem;
  }

  p {
    font-size: 1.3rem;
    margin-top: 1rem;
  }
}
</style>
