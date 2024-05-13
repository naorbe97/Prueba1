<template>
  <div>
    <HeaderImage :source="'/image1.jpg'" />
    <main class="container">
      <h1>{{ title }}</h1>
      <p>
        Lorem Ipsum es simplemente el texto de relleno de las imprentas y
        archivos de texto. Lorem Ipsum ha sido el texto de relleno estándar de
        las industrias desde el año 1500, cuando un impresor (N. del T. persona
        que se dedica a la imprenta) desconocido usó una galería de textos y los
        mezcló de tal manera que logró hacer un libro de textos especimen. No
        sólo sobrevivió 500 años, sino que tambien ingresó como texto de relleno
        en documentos electrónicos, quedando esencialmente igual al original.
      </p>
    </main>
    <section class="container card-section">
      <article-card v-for="(item, index) in 4" :key="index" />
    </section>
  </div>
</template>

<style lang="postcss">
.card-section {
  display: flex;
  justify-content: space-between;
}
</style>

<script setup>
import { ref } from "vue";
const title = ref("Home");
const articles = ref([
 {
  id:1,
  title: "Articulo 1",
  url: "/image3.jpg"
},
{
  id:1,
  title: "Articulo 2",
  url: "/image4.jpg"
},
{
  id:1,
  title: "Articulo 3",
  url: "/image5.jpg"
},
{
  id:1,
  title: "Articulo 4",
  url: "/image6.jpg"
},
])
</script>
