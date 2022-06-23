<template>
      <div class="category-boxes">
            <div class="col-5 d-flex align-items-center justify-content-start">
                  <a :href="categoryAddress" class="text-black p-4">
                        <span class="category-text ps-1"> {{ categoryText }} </span>
                  </a>
            </div>
            <div class="flesh-svg d-flex align-items-center justify-content-center">
                  <img src="../../assets/svg/Flesh.svg" alt="" />
            </div>
            <div class="col-5 d-flex align-items-center justify-content-end">
                  <img :src="require(`../../assets/images/${categoryImage}`)" alt="" />
            </div>
      </div>
</template>

<script>
export default {
      props: {
            categoryText: {
                  type: String,
                  required: true,
            },
            categoryAddress: {
                  type: String,
                  required: true,
            },
            categoryImage: {
                  required: true,
            },
      },
      data() {
            return {};
      },
};
</script>

<style lang="scss">
.category-boxes {
      display: flex;
      background-color: #eeebe6;
      height: 115px;
      a {
            text-decoration: none !important;
      }
      .category-text {
            font-weight: 400;
            font-size: 18px;
            line-height: 23px;
      }
      .flesh-svg {
            img {
                  width: 15px;
                  height: 15px;
            }
      }
}
</style>
