<template>
  <section class="flex q-pa-lg bg-dark justify-center">
    <div class="q-pa-lg">
      <h1 class="text-h4 text-info text-raleway q-pt-xl">Reformas</h1>
      <p class="size-18 text-montserrat-400">
        Nossa empresa de piscinas oferece reformas personalizadas,
        <br />
        incluindo a troca de azulejos sem esvaziar a piscina.
      </p>
      <p class="size-18 text-montserrat-400">
        Priorizamos a eficiência e a sustentabilidade, com expertise
        <br />
        em modernização de sistemas e renovação de revestimentos,
        <br />
        garantindo resultados de alta qualidade
      </p>
    </div>

    <div class="q-pa-md q-mt-xl">
      <img src="img/img-servico1.webp" alt="" />
    </div>
  </section>

  <section  class="aaa flex q-pa-lg justify-center">
  <div class="q-pa-lg text-right">
    <h1 class="text-h4 text-info text-raleway q-pt-xl">Vazamento</h1>
    <p class="size-18 text-montserrat-400">
      Serviço de
      <span class="text-bold">reparo hidráulico, precedido de visita técnica</span>
      <br />
      para detecção de vazamento com investigação a partir do
      <br />
      hidrômetro.
    </p>
  </div>
  <div class="q-pa-md q-mt-xl">
    <img src="img/img-servico2.webp" alt="" />
  </div>
</section>


  <section class="flex q-pa-lg bg-dark justify-center">
    <div class="q-pa-lg">
      <h1 class="text-h4 text-info text-raleway q-pt-xl">Pintura de Piscinas</h1>
      <p class="size-18 text-montserrat-400">
        A Golfim Piscinas trabalha na área de
        <span class="text-bold">pintura e reformas</span>
        <br />
        <span class="text-bold">de piscinas de fibra</span>
        , atendendo seu cliente com respeito
        <br />
        e qualidade. Utilizamos os melhores produtos do mercado
        <br />
        para executar um serviço de excelência, com profissionais
        <br />
        capacitados garantindo a satisfação de nosso cliente.
      </p>
    </div>

    <div class="q-pa-md q-mt-xl">
      <img src="img/img-servico3.webp" alt="" />
    </div>
  </section>
</template>

<script setup></script>

<style lang="scss" scoped>
img {
  border-radius: 10px;
  width: 26rem;
  height: 16rem;
  border: 1px solid black;
}
.aaa{
  flex-direction: row-reverse;

  @media screen and (max-width: 600px) {
    flex-direction: rom;
  }
} 
</style>
