<script setup lang="ts">
import ButtonPrimary from "@/components/_ui/ButtonPrimary.vue";
import InputBase from "@/components/form/InputBase.vue";
</script>

<template>
<div class="flex w-full h-screen bg-gray-900 flex-col">
  <div class="flex justify-end items-center gap-2">
    <ButtonPrimary title="Server"></ButtonPrimary>
    <ButtonPrimary title="?"></ButtonPrimary>
    <ButtonPrimary title="?"></ButtonPrimary>
  </div>
  <div class="flex justify-center items-center flex-col gap-4 h-screen">
    <InputBase label="test" placeholer="placeholer" ></InputBase>

    <h1 class="bold text-green-700  text-shadow-lg text-shadow-lime-200 text-7xl font-stretch-expanded tracking-wide" >LEANCRAFT</h1>
    <span class="text-green-300 text-2xl"> Subtitle</span>
  </div>
</div>
</template>
