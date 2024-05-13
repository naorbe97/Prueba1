<template>
  <img class="header-image" :src="source" alt="Imagen de cabecera" />
</template>

<style lang="postcss">
.header-image {
  width: 100%;
  height: 250px;
  object-fit: cover;
}
</style>

<script setup>
const props = defineProps({
  source: {
    type: String,
    requiered: false,
  },
});
const { source } = props;
</script>
