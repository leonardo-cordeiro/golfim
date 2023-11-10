<template>
  <div class="wrap">
    <div class="content">
      <div class="flex q-mr-xl">
        <h1 class="text-h3 text-info text-raleway">
          Troca de azulejos
          <span style="text-decoration: underline">
            <br />
            sem esvaziar
            <br />
            a piscina
          </span>
        </h1>
        <p class="size-18 text-montserrat-400">
          Para evitar desperdício de água, a troca de
          <br />
          azulejos para piscinas sem esvaziá-la é uma
          <br />
          ótima solução
        </p>
        <p class="size-18 q-mt-lg q-pt-lg text-montserrat-400">
          Esse processo de fazer a troca de azulejos para
          <br />
          piscinas, sem esvaziá-la é necessário ter larga
          <br />
          experiência e treinamento como nós!
        </p>
        <p class="text-montserrat text-bold size-16 text-left flex no-wrap items-center q-ml-lg">
          <q-icon name="verified" size="lg" color="info" />
          <span class="q-ml-sm">
            A troca de azulejos para piscinas é feita por
            <br />
            mergulhadores profissionais treinados.
          </span>
        </p>

        <p class="text-montserrat text-bold size-16 text-left flex no-wrap items-center q-ml-lg">
          <q-icon name="verified" size="lg" color="info" />
          <span class="q-ml-sm">
            Logo após a conclusão do trabalho, a piscina
            <br />
            já está liberada para uso normal.
          </span>
        </p>

        <q-btn class="q-ml-xl q-my-md" rounded color="info">
          Quer saber como isso funciona?
          <br />
          Fale Conosco
        </q-btn>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.wrap {
  height: 100%;
  width: 100%;
  background: url('/img/background-2.webp?');
  background-repeat: no-repeat;
  background-size: cover;
  object-fit: cover;
  display: flex;
  flex-direction: column;

  .content {
    text-align: right;
    margin-left: 50%;
    width: 50%;
    h1 {
      line-height: 5rem;
    }
  }
  @media screen and (max-width: 600px) {
    background-position:  center;
    .content {
      margin-left: 10%;
      width: 90%; //
    }
   
  }
}
</style>
