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
          :medium="$vuetify.breakpoint.smAndBelow"
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
          <div class="cont-box--icon">
            <ion-icon name="book"></ion-icon>
          </div>
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
          <div class="cont-box--icon">
            <ion-icon name="shapes"></ion-icon>
          </div>
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
          <div class="cont-box--icon">
            <ion-icon name="construct"></ion-icon>
          </div>
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
      <div class="action">
        <v-btn
          tile
          light
          :large="$vuetify.breakpoint.mdAndUp"
          :medium="$vuetify.breakpoint.smAndBelow"
          elevation="4"
          class="my-btn join-btn"
        >
          <h1>Join Us</h1>
        </v-btn>
      </div>
    </section>
  </v-layout>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
#first-page {
  margin-bottom: max(50px, 6vw);
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
    display: flex;
    flex-direction: row;
    margin: 5rem 0;
    @media (max-width: 900px) {
      flex-direction: column;
    }

    &-box {
      height: 300px;
      width: 250px;
      margin: 2rem 2vw;
      border: 3px solid #fff;
      border-radius: 25px 25px 10px 10px;
      display: grid;
      grid-template-rows: 250px 45px;
      position: relative;
      opacity: 0.8;
      transition: all 0.1s ease;

      &:hover {
        opacity: 1;
      }

      &--icon {
        position: absolute;
        top: -5%;
        right: -5%;
        padding: 5px;
        background-color: #2c2c2c;
        ion-icon {
          font-size: 7rem;
        }
      }

      &--body {
        padding: 50px 25px;
        font-size: 16px;
        text-align: left;
        line-height: 1.2;
        font-weight: 400;
      }
      &--title {
        background-color: #fff;
        color: #444;
        display: flex;
        justify-content: center;
        align-items: center;
        span {
          font-weight: 500;
          font-size: 3rem;
        }
      }
    }
  }
}
</style>
