<template>
      <Header />
      <HeaderPicture />
      <ProductCategory />
      <div class="bg-black text-white px-5 py-3">
            <LatestNews />
      </div>
</template>

<script>
import Header from "./components/Custom-Header.vue";
import HeaderPicture from "./components/Header-Picture.vue";
import ProductCategory from "./components/categories/Product-category.vue";
import LatestNews from "./components/latest-news/Latest-News.vue";

export default {
      name: "App",
      components: {
            Header,
            HeaderPicture,
            ProductCategory,
            LatestNews,
      },
};
</script>

<style>
#app {
      font-family: Avenir, Helvetica, Arial, sans-serif;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
}
* {
      margin: 0;
      padding: 0;
      outline: none;
      text-decoration: none;
      list-style-type: none;
      box-sizing: border-box;
      text-transform: capitalize !important;
}
</style>
