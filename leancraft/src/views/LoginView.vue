<script setup lang="ts">

</script>

<template>
<div class=" border border-green-700 rounded-md p-4 w-full max-w-sm mx-auto">
  <h1 class="text-2xl text-center text-green-700">Login</h1>
  <form class="flex flex-col gap-4">
    <InputText label="Email" type="email" name="email" id="email" placeholder="Enter your email" required />
    <InputText label="Password" type="password" name="password" id="password" placeholder="Enter your password" required />
    <ButtonBase type="submit" label="Login" />
  </form>
</template>

<style scoped>

</style>
