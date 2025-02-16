<template>
  <div class="pb-4">

    <section class="relative h-fit">
      <img :src="HeroMobile" alt="Logo" class="w-full" />

      <div class="bg-[#FFF3E3] rounded-l p-2 max-w-60 absolute bottom-0 right-0">
        <h1 class="text-sm font-semibold text-[#B88E2F]/80 pb-2">Transforme suas ideias em produtos únicos
        </h1>
        <h2 class="hidden md:block">Descubra a magia da papelaria feita sob medida para você. Cada detalhe pensado para
          encantar e satisfazer
          suas
          expectativas!</h2>

        <button class="bg-[#B88E2F] p-2 rounded text-white text-sm">Personalize Agora</button>
      </div>
    </section>

    <section class="px-4">
      <h1 class="text-2xl font-semibold text-[#B88E2F] py-4">Conheça nossos produtos</h1>
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
        <div class="bg-[#FFF3E3] rounded p-4">
          <h2 class="text-lg font-semibold text-[#B88E2F]">Caderno de Anotações</h2>
          <p class="text-sm">Caderno de anotações com capa dura e folhas pautadas. Ideal para anotar suas ideias e
            pensamentos.</p>
          <button class="bg-[#B88E2F] p-2 rounded text-white text-sm">Personalize Agora</button>
        </div>
        <div class="bg-[#FFF3E3] rounded p-4">
          <h2 class="text-lg font-semibold text-[#B88E2F]">Agenda</h2>
          <p class="text-sm">Descrição</p>
          <button class="bg-[#B88E2F] p-2 rounded text-white text-sm">Personalize Agora</button>
        </div>
        <div class="bg-[#FFF3E3] rounded p-4">
          <h2 class="text-lg font-semibold text-[#B88E2F]">Adesivos Personalizados</h2>
          <p class="text-sm">Descrição.</p>
          <button class="bg-[#B88E2F] p-2 rounded text-white text-sm">Personalize Agora</button>
        </div>
      </div>
    </section>

    <section>
      <h1 class="text-2xl font-semibold text-[#B88E2F] py-4">Produtos mais vendidos</h1>
    </section>


  </div>
</template>

<script lang="ts" setup>
import HeroMobile from '@/assets/images/hero-mobile.png';
</script>

<style></style>