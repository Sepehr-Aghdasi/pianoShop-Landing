<template>
      <div class="featured-products">
            <div class="d-flex mb-5">
                  <span class="custom-line mx-lg-5 mx-1"></span>
                  <h2 class="h1 fw-bold" style="white-space: nowrap">featured products</h2>
                  <span class="custom-line mx-lg-5 mx-1"></span>
            </div>
            <div class="row">
                  <div class="col-lg-3 col-md-6 col-12 mb-4">
                        <FeaturedProductBox
                              :imageUrl="featuredProductArray[0].imageUrl"
                              :title="featuredProductArray[0].title"
                              :description="featuredProductArray[0].description"
                              :price="featuredProductArray[0].price"
                              :url="featuredProductArray[0].url"
                        />
                  </div>
                  <div class="col-lg-6 col-12 mb-4">
                        <ImageBox
                              :imageUrl="imageBoxProperty.imageUrl"
                              :title="imageBoxProperty.title"
                              :description="imageBoxProperty.description"
                              :price="imageBoxProperty.price"
                              :url="imageBoxProperty.url"
                        />
                  </div>
                  <div class="col-lg-3 col-md-6 col-12 mb-4">
                        <FeaturedProductBox
                              :imageUrl="featuredProductArray[1].imageUrl"
                              :title="featuredProductArray[1].title"
                              :description="featuredProductArray[1].description"
                              :price="featuredProductArray[1].price"
                              :url="featuredProductArray[1].url"
                        />
                  </div>
                  <div
                        v-for="(item, index) in featuredProductArray.slice(2)"
                        :key="index"
                        class="col-lg-3 col-md-6 col-12 mb-4"
                  >
                        <FeaturedProductBox
                              :imageUrl="item.imageUrl"
                              :title="item.title"
                              :description="item.description"
                              :price="item.price"
                              :url="item.url"
                        />
                  </div>
                  <div class="seeAll-button d-flex justify-content-center mt-5">
                        <span class="custom-line"></span>
                        <button
                              class="btn border border-dark px-4"
                              style="border-radius: 0 !important; white-space: nowrap"
                        >
                              see all
                              <img
                                    src="../../assets/svg/Right-ARROW-black.svg"
                                    class="ps-2"
                                    alt=""
                              />
                        </button>
                        <span class="custom-line"></span>
                  </div>
            </div>
      </div>
</template>

<script>
import FeaturedProductBox from "./Featured-Product-Box.vue";
import ImageBox from "./Image-Box.vue";

export default {
      components: { FeaturedProductBox, ImageBox },
      data() {
            return {
                  imageBoxProperty: {
                        imageUrl: "Rectangle-18.png",
                        title: "STEINWAY & SONS",
                        description: "UPRIGHT PIANO MODEL K – C2003",
                        price: "£36,995",
                        url: "#",
                  },
                  featuredProductArray: [
                        {
                              id: 0,
                              imageUrl: "Yamaha.png",
                              title: "YAMAHA",
                              description: "P121 UPRIGHT PIANO – C2013",
                              price: "£6,295.00",
                              url: "#",
                        },
                        {
                              id: 1,
                              imageUrl: "WELMAR-MODEL-126-1.png",
                              title: "WELMAR",
                              description: "126 UPRIGHT PIANO – C2000",
                              price: "£8,995.00",
                              url: "#",
                        },
                        {
                              id: 2,
                              imageUrl: "SCHIMMEL-122-1.png",
                              title: "SCHIMMEL",
                              description: "122 UPRIGHT PIANO – C1998",
                              price: "£12,995.00",
                              url: "#",
                        },
                        {
                              id: 3,
                              imageUrl: "BOSENDORFER-170-1.png",
                              title: "BOSENDORFER",
                              description: "170 GRAND PIANO – C2008",
                              price: "£56,995.00",
                              url: "#",
                        },
                        {
                              id: 4,
                              imageUrl: "STEINWAY-ESSEX-116-1.png",
                              title: "STEINWAY",
                              description: "ESSEX 116 UPRIGHT PIANO",
                              price: "£4,995.00",
                              url: "#",
                        },
                        {
                              id: 5,
                              imageUrl: "JOHN-BROADWOOD.png",
                              title: "JOHN BROADWOOD AND SONS",
                              description: "GRAND PIANO – C1925",
                              price: "£14,995.00",
                              url: "#",
                        },
                  ],
            };
      },
};
</script>

<style lang="scss">
.featured-products {
      .custom-line {
            border-bottom: 1px solid rgba(0, 0, 0, 0.8);
            display: flex;
            width: 40%;
            margin-bottom: 25px;
      }
      .seeAll-button {
            .custom-line {
                  border-bottom: 1px solid rgba(0, 0, 0, 0.8);
                  display: flex;
                  width: 100%;
                  margin-bottom: 17px;
            }
      }
}
</style>
