<template>
      <div class="d-flex">
            <span class="custom-line mx-lg-5 mx-1"></span>
            <h2 class="h2" style="white-space: nowrap">featured products</h2>
            <span class="custom-line mx-lg-5 mx-1"></span>
      </div>
      <div class="row">
            <div class="col-3">
                  <FeaturedProductBox />
            </div>
            <div class="col-3">
                  <FeaturedProductBox />
            </div>
            <div class="col-3">
                  <FeaturedProductBox />
            </div>
            <div class="col-3">
                  <FeaturedProductBox />
            </div>
      </div>
</template>

<script>
import FeaturedProductBox from "./Featured-Product-Box.vue";

export default {
      components: { FeaturedProductBox },
      data() {
            return {
                  FeaturedProductArray: [
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

<style>
.custom-line {
      border-bottom: 1px solid rgba(0, 0, 0, 0.8);
      display: flex;
      width: 40%;
      margin-bottom: 25px;
}
</style>
