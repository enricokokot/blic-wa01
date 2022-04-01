<template>
  <div class="about">
    <router-link to="/"><h1>This is a back button</h1></router-link>
    <p>Name: {{ book.name }}</p>
    <p>Authors: {{ book.authors }}</p>
    <p>ISBN: {{ book.isbn }}</p>
    <p>Pages: {{ book.numberOfPages }}</p>
    <p>Publisher: {{ book.publisher }}</p>
    <p>Country: {{ book.country }}</p>
    <p>Number of characters: {{ book.characters.length }}</p>
  </div>
</template>

<script>
import store from "@/store";

export default {
  name: "AboutView",
  data: () => ({
    book: store.currentBook,
  }),
};
</script>
