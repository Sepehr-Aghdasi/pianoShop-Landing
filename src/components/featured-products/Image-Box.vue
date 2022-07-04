<template>
      <div class="image-box card bg-dark text-white">
            <img :src="require(`../../assets/images/${imageUrl}`)" class="card-img" alt="" />
            <a :href="url">
                  <div class="card-img-overlay">
                        <h5 class="card-title">{{ title }}</h5>
                        <p class="card-text">
                              {{ description }}
                        </p>
                        <p class="card-text">{{ price }}</p>
                  </div>
            </a>
      </div>
</template>

<script>
export default {
      props: {
            imageUrl: {
                  type: String,
                  required: true,
            },
            title: {
                  type: String,
                  required: true,
            },
            description: {
                  type: String,
                  required: true,
            },
            price: {
                  type: String,
                  required: true,
            },
            url: {
                  type: String,
                  required: true,
            },
      },
};
</script>

<style lang="scss">
.image-box {
      .card-img {
            background: black;
            overflow: hidden;
            object-fit: cover;
            opacity: 0.4;
      }
}
</style>
