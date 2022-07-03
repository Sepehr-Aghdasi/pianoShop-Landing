<template>
      <div class="card featured-Product-card p-3">
            <a :href="url">
                  <img
                        :src="require(`../../assets/images/${imageUrl}`)"
                        class="card-img-top"
                        alt=""
                  />
            </a>
            <div class="card-body text-center">
                  <h4 class="card-title text-muted fs-6">{{ title }}</h4>
                  <p class="card-text fw-bold">{{ description }}</p>
                  <p class="text-muted m-0">{{ price }}</p>
            </div>
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

<style scoped>
.featured-Product-card {
      border-top: 1px solid rgba(0, 0, 0, 1) !important;
      border-right: 1px solid rgba(0, 0, 0, 0.6) !important;
      border-left: 1px solid rgba(0, 0, 0, 0.6) !important;
      border-bottom: 1px solid rgba(0, 0, 0, 0.6) !important;
      border-radius: 0 !important;
}
.card-text,
.card-title {
      white-space: nowrap !important;
}
</style>
