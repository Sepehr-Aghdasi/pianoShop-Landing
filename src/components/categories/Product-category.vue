<template>
      <div class="categories-area">
            <span class="custom-line mx-lg-5 mx-1"></span>
            <h3 class="text-center m-0">Categories</h3>
            <span class="custom-line mx-lg-5 mx-1"></span>
      </div>
      <div class="row justify-content-evenly">
            <ProductCategoryBox
                  v-for="item in categoryArray"
                  :key="item.id"
                  :categoryText="item.title"
                  :categoryImage="item.imageUrl"
                  :categoryAddress="item.address"
                  class="col-lg-3 col-md-6 col-12 m-3"
            />
      </div>
      <div class="seeAll-button d-flex justify-content-center">
            <span class="custom-line"></span>
            <button
                  class="btn border border-dark px-4"
                  style="border-radius: 0 !important; white-space: nowrap"
            >
                  see all
                  <img src="../../assets/svg/Right-ARROW-black.svg" class="ps-2" alt="" />
            </button>
            <span class="custom-line"></span>
      </div>
</template>

<script>
import ProductCategoryBox from "./Product-category-box.vue";

export default {
      components: {
            ProductCategoryBox,
      },
      data() {
            return {
                  categoryArray: [
                        {
                              id: 0,
                              imageUrl: "Accessories.png",
                              title: "Accessories",
                              address: "#",
                        },
                        {
                              id: 1,
                              imageUrl: "Spinet-Piano.png",
                              title: "Spinet Pianos",
                              address: "#",
                        },
                        {
                              id: 2,
                              imageUrl: "Digital-Piano.png",
                              title: "Digital Pianos",
                              address: "#",
                        },
                        {
                              id: 3,
                              imageUrl: "Upright-Piano.png",
                              title: "Upright Pianos",
                              address: "#",
                        },
                        {
                              id: 4,
                              imageUrl: "Grand-Piano.png",
                              title: "Grand Pianos",
                              address: "#",
                        },
                        {
                              id: 5,
                              imageUrl: "Studio-Piano.png",
                              title: "Studio Pianos",
                              address: "#",
                        },
                  ],
            };
      },
};
</script>

<style lang="scss">
.categories-area {
      margin: 50px 0;
      display: flex;
      justify-content: center;
      h3 {
            font-weight: 600;
            font-size: 38px;
            line-height: 48px;
            text-align: center;
            letter-spacing: 0.02em;
            overflow: hidden;
      }
      span {
            border-bottom: solid #000 2px;
            display: flex;
            width: 15%;
            margin-bottom: 23px;
      }
}
.seeAll-button {
      .custom-line {
            border-bottom: 1px solid rgba(0, 0, 0, 0.8);
            display: flex;
            width: 40%;
            align-items: center;
            justify-content: center;
            margin-bottom: 17px;
      }
}
</style>
