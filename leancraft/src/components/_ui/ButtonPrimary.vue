<script setup lang="ts">

import {computed} from "vue";
import Icon from "@/components/Icon.vue";

const props = defineProps<{
  title: string,
  type?: string,
  ariaLabel?: string,
  iconPrefix?:  string,
  iconPostfix?: string,
}>()

const ariaLabel = computed(() => props.ariaLabel || props.title)
const emit = defineEmits(['click'])
const click = () => {
  emit('click')
}
</script>

<template>
  <button
    @click="click"
    :ariaLabel="ariaLabel"
    class="appearance-none text-white bg-gradient-to-r from-green-500 via-green-600 to-green-700 hover:bg-gradient-to-br focus:ring-4
    focus:outline-none focus:ring-green-300 dark:focus:ring-green-800 shadow-lg shadow-green-500/50 dark:shadow-lg dark:shadow-green-800/80
    font-medium rounded-lg text-sm px-5  py-2 text-center me-2 mb-2" >
    <slot name="icon-prefix">
      <icon v-if="iconPrefix" name="props.iconPrefix" class="w-4 h-4 mr-2"></icon>
    </slot>
    {{title}}
    <slot name="icon-postfix"></slot>
  </button>
</template>



<style scoped>

</style>
