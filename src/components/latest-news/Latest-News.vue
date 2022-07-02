<template>
      <div class="p-3">
            <div class="mx-3 mb-5">
                  <div class="d-flex justify-content-between align-items-center col-12">
                        <div class="d-flex align-items-center col-6">
                              <span class="custom-line me-3"></span>
                              <h2 class="mb-0 display-5">latest news</h2>
                        </div>
                        <div class="col-6 d-flex justify-content-end align-items-center h-100">
                              <a href="#">
                                    <p
                                          class="m-0"
                                          style="color: rgba(255, 255, 255, 0.8) !important"
                                    >
                                          view all
                                          <img src="../../assets/svg/Right-ARROW.svg" alt="" />
                                    </p>
                              </a>
                        </div>
                  </div>
                  <hr class="bg-white" />
            </div>
            <div class="row col-12 m-0">
                  <LatestNewsBox
                        v-for="(item, index) in newsArray"
                        :key="index"
                        :title="item.title"
                        :description="item.description"
                        :imageUrl="item.imageUrl"
                        :url="item.url"
                        class="col-lg-4 col-md-6 col-12"
                  />
            </div>
      </div>
</template>

<script>
import LatestNewsBox from "./Latest-News-Box.vue";

export default {
      components: { LatestNewsBox },
      data() {
            return {
                  newsArray: [
                        {
                              id: 0,
                              title: "event",
                              description:
                                    "World International Piano Competition 2022 Starts This Month",
                              imageUrl: "Rectangle-13.png",
                              url: "#",
                        },
                        {
                              id: 1,
                              title: "event",
                              description: "Butterfly Pianos and Symmetrical Grands",
                              imageUrl: "Rectangle-14.png",
                              url: "#",
                        },
                        {
                              id: 0,
                              title: "event",
                              description:
                                    "The Appassionata — Steinway Celebrates Beethoven’s 250th Birthday",
                              imageUrl: "Rectangle-15.png",
                              url: "#",
                        },
                  ],
            };
      },
};
</script>

<style>
.custom-line {
      border-bottom: 1px solid #fff;
      display: flex;
      width: 8%;
}
</style>
