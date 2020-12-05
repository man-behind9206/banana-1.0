<template>
  <v-layout column justify-center align-center text-center>
    <section id="first-page">
      <div class="first-page--image my-2 my-sm-5">
        <img src="/DSC_cover.png" alt="DSC Cover" />
      </div>
      <div class="first-page--actions py-1 py-lg-5">
        <v-btn
          tile
          light
          :large="$vuetify.breakpoint.mdAndUp"
          :medium="$vuetify.breakpoint.sm"
          :small="$vuetify.breakpoint.xs"
          elevation="4"
          class="my-btn explore-btn"
        >
          <h1>Explore Now</h1>
        </v-btn>
      </div>
    </section>

    <section id="who-are-we">
      <div class="head">
        <h1 class="head_text">Who Are We?</h1>
        <p class="head_desc desc">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quidem sint
          excepturi recusandae possimus dolores eos aspernatur nemo delectus
          illum voluptates corrupti corporis adipisci eveniet eius porro unde,
          maiores placeat laborum.
        </p>
      </div>
      <div class="cont">
        <div class="cont-box cont-box-1">
          <div class="cont-box--body">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud.
            </p>
          </div>
          <div class="cont-box--title">
            <span>Study</span>
          </div>
        </div>
        <div class="cont-box cont-box-2">
          <div class="cont-box--body">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud.
            </p>
          </div>
          <div class="cont-box--title">
            <span>Analyze</span>
          </div>
        </div>
        <div class="cont-box cont-box-3">
          <div class="cont-box--body">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud.
            </p>
          </div>
          <div class="cont-box--title">
            <span>Solve</span>
          </div>
        </div>
      </div>
    </section>
  </v-layout>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
#first-page {
  margin-bottom: max(24px, 5vw);
  .first-page--image {
    img {
      width: max(80%, 60vw);
      @media (min-width: 1900px) {
        width: 60vw;
      }
    }
  }
}

#who-are-we {
  display: flex;
  flex-direction: column;
  align-items: center;
  .head {
    max-width: 900px;
    margin: 0 25px;
  }
  .cont {
    &-box {
      height: 300px;
      width: 250px;
      border: 3px solid #fff;

      &-body {
      }
      &-title {
      }
    }
    &-box-1 {
    }
    &-box-2 {
    }
    &-box-3 {
    }
  }
}
</style>
