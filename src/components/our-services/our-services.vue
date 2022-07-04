<template>
      <div class="services">
            <div class="our-services mb-5">
                  <span class="custom-line mx-lg-5 mx-1"></span>
                  <h2 class="h1 fw-bold text-center m-0">our services</h2>
                  <span class="custom-line mx-lg-5 mx-1"></span>
            </div>
            <div class="row">
                  <div class="col-lg-6 col-12">
                        <img
                              class="col-12"
                              src="../../assets/images/Our-Services-Picture.png"
                              alt=""
                        />
                  </div>
                  <div class="col-lg-6 col-12">
                        <div
                              class="d-flex flex-column justify-content-evenly align-items-center px-lg-5 px-2 h-100 mt-lg-0 mt-3"
                        >
                              <h3 class="h1">Piano Tuning</h3>
                              <p class="text-center text-lowercase">
                                    With over 260 strings a fine piano requires regular tuning, to
                                    consistently perform at its optimum standard. We recommend your
                                    piano is tuned at least twice a year, and quarterly if you are a
                                    professional pianist or piano teacher...
                              </p>
                              <button
                                    class="btn btn-light border border-dark px-4 py-2 mb-3"
                                    style="border-radius: 0 !important"
                              >
                                    Find Out More
                                    <img
                                          class="ps-2"
                                          src="../../assets/svg/Right-ARROW-black.svg"
                                          alt=""
                                    />
                              </button>
                              <div class="circle-box">
                                    <span></span>
                                    <span></span>
                                    <span></span>
                              </div>
                        </div>
                  </div>
            </div>
      </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.services {
      .our-services {
            display: flex;
            justify-content: center;
            .custom-line {
                  border-bottom: solid #000 1px;
                  display: flex;
                  width: 30%;
                  margin-bottom: 17px;
            }
      }
      .circle-box {
            display: flex;
            span {
                  width: 12px;
                  height: 12px;
                  border: 1px solid rgba(0, 0, 0, 0.8);
                  border-radius: 100%;
                  margin: 0 10px;
                  &:nth-child(1) {
                        background-color: #000;
                  }
            }
      }
}
</style>
