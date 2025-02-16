<template>
  <div class="w-full flex justify-between gap-4 md:grid md:grid-cols-[20%_60%_20%] items-center p-4 bg-white">

    <Menu class="md:hidden w-10 h-10" @click="toggleMenuBar" />

    <NuxtLink to="/" class="text-bold text-4xl text-center">AGP</NuxtLink>

    <div class="w-full">
      <input type="text" placeholder="Pesquisar ..." class="border border-gray-300 rounded-lg p-2 w-full" />
    </div>

    <div class="hidden md:flex items-center justify-center space-x-8">
      <ShoppingCart />
      <User />
    </div>

    <div v-if="isMenuBarOpen" class="md:hidden fixed top-0 left-0 w-3/4 h-full bg-white z-50">

      <div class="flex justify-end p-4">
        <X class="w-10 h-10" @click="toggleMenuBar" />
      </div>

      <div>
        <div>
          <CircleUserRound class="w-20 h-20 mx-auto" />
          <p class="text-center">Olá, visitante</p>
        </div>
      </div>

      <div class="flex justify-center pt-4">
        <div class="w-4/5 h-[2px] bg-gray-200 px-4"></div>
      </div>

      <div>
        <div>

          <NuxtLink to="/" class="flex items-center justify-start space-x-4 p-4">
            <House />
            <p>Página inicial</p>
          </NuxtLink>

          <NuxtLink to="/" class="flex items-center justify-start space-x-4 p-4">
            <ShoppingCart />
            <p>Meu carrinho</p>
          </NuxtLink>

          <NuxtLink to="/" class="flex items-center justify-start space-x-4 p-4">
            <User />
            <p>Minha conta</p>
          </NuxtLink>
        </div>
      </div>

    </div>

  </div>
</template>

<script lang="ts" setup>
import { ShoppingCart, User, Menu, CircleUserRound, X, House } from 'lucide-vue-next';

const isMenuBarOpen = ref(false);

const toggleMenuBar = () => {
  isMenuBarOpen.value = !isMenuBarOpen.value;
}
</script>

<style></style>