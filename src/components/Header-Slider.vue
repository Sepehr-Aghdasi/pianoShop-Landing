<template>
      <div class="col-12">
            <div class="header-image">
                  <div class="header-pic-text h-100">
                        <p class="m-0 text-center">Welcome to</p>
                        <p class="m-0 text-center">Antique Piano Shop</p>
                  </div>
            </div>
      </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.header-image {
      width: 100%;
      height: 512px;
      background-image: url("../assets/images/HeaderPic.png");
      background-repeat: no-repeat;
      background-position: center center;
      -webkit-background-size: cover;
      background-size: cover;
      .header-pic-text {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            p {
                  font-weight: 600;
                  font-size: 50px;
                  line-height: 102px;
                  text-align: center;
                  letter-spacing: -0.03em;
                  color: #fff;
            }
      }
}
</style>
