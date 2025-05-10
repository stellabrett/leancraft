<script setup lang="ts">
type Props = {
  placeholder?: string
  type?: string
  name?: string
  id?: string
  label?: string
  required?: boolean
  ariaLabel?: string
}
const props = defineProps<Props>()
const model = defineModel()
</script>

<template>
  <div class="flex justify-start items- start flex-col gap-2">
    <label class="text-sm text-green-700" :for="props.id" :aria-label="props.ariaLabel || props.label">{{ props.label }}</label>

    <input class="border border-green-700 rounded-md p-2 w-full"
           :placeholder="props.placeholder"
           :type="props.type"
           :name="props.name"
           :id="props.id"
           v-model="model" />
  </div>

</template>

<style scoped>

</style>
