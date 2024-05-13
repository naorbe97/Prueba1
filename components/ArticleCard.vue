<template>
  <article>
    <img src="article.url" alt="article.tittle" />
    <button>{{ article.title }}</button>
  </article>
</template>

<script setup>
const props = defineProps({
  article: {
    type: Object,
    required: false,
  },
});
const { article } = props;
</script>

<style lang="postcss">
article {
  @apply w-1/5 m-20;
  img {
    @apply h-32;
    object-fit: cover;
  }
  button {
    @apply p-5 bg-gray-200 w-32;
    text-align: center;
  }
}
</style>
