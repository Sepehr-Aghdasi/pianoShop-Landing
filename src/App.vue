<template>
      <Header />
      <HeaderPicture />
      <div class="m-5">
            <ProductCategory />
      </div>
      <div class="bg-black text-white p-5">
            <LatestNews />
      </div>
      <div class="m-5">
            <FeaturedProduct />
      </div>
      <div class="m-5">
            <OurServices />
      </div>
      <CustomFooter />
</template>

<script>
import Header from "./components/Custom-Header.vue";
import HeaderPicture from "./components/Header-Slider.vue";
import ProductCategory from "./components/categories/Product-category.vue";
import LatestNews from "./components/latest-news/Latest-News.vue";
import FeaturedProduct from "./components/featured-products/Featured-Product.vue";
import OurServices from "./components/our-services/our-services.vue";
import CustomFooter from "./components/footer/Custom-Footer.vue";

export default {
      name: "App",
      components: {
            Header,
            HeaderPicture,
            ProductCategory,
            LatestNews,
            FeaturedProduct,
            OurServices,
            CustomFooter,
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
a {
      color: inherit !important;
      text-decoration: none !important;
}
</style>
