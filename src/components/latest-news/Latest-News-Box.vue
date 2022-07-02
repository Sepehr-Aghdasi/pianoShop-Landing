<template>
      <div class="card bg-black">
            <a :href="url">
                  <img
                        :src="require(`../../assets/images/${imageUrl}`)"
                        class="card-img-top"
                        alt=""
                  />
            </a>
            <div class="card-body px-0">
                  <h5 class="card-title text-muted text-uppercase">{{ title }}</h5>
                  <p class="card-text fs-5">
                        {{ description }}
                  </p>
            </div>
      </div>
</template>

<script>
export default {
      props: {
            title: {
                  type: String,
                  required: true,
            },
            description: {
                  type: String,
                  required: true,
            },
            imageUrl: {
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

<style></style>
