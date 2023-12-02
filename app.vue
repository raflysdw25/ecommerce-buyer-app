<template>
  <h1 class="text-3xl font-bold underline">Hello world!</h1>
</template>
<script setup>
const { $sentryCaptureException } = useNuxtApp();

onMounted(() => {
  $sentryCaptureException("Sentry Buyer App Exception");
});
</script>
