<template>
  <v-app dark>
    <v-navigation-drawer v-model="rightDrawer" right fixed width="100%">
      <v-btn icon absolute top right @click="closeDrawer" class="pa-2">
        <v-icon @click="rightDrawer = false" x-large>mdi-close</v-icon>
      </v-btn>
      <div class="nav_links">
        <ul>
          <li><NuxtLink to="/">HOME</NuxtLink></li>
          <li><NuxtLink to="/about" prefetch>ABOUT</NuxtLink></li>
          <li><NuxtLink to="/live">LIVE</NuxtLink></li>
          <li><NuxtLink to="/team">TEAM</NuxtLink></li>
          <li><NuxtLink to="/opinion">OPINION</NuxtLink></li>
        </ul>
      </div>
    </v-navigation-drawer>
    <v-app-bar app>
      <!-- <v-toolbar-title v-text="title" /> -->

      <img
        src="~/assets/DSC-NITR.png"
        alt="DSC NITR Logo"
        :height="
          $vuetify.breakpoint.xs
            ? '24px'
            : $vuetify.breakpoint.sm
            ? '32px'
            : '40px'
        "
      />
      <v-spacer />
      <v-btn icon>
        <v-icon
          @click.stop="rightDrawer = true"
          :large="$vuetify.breakpoint.sm"
          :x-large="$vuetify.breakpoint.mdAndUp"
          >mdi-menu</v-icon
        >
      </v-btn>
    </v-app-bar>
    <v-main>
      <v-container>
        <nuxt />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      title: 'Vuetify.js',
      rightDrawer: false,
    }
  },
  methods: {
    closeDrawer() {
      console.log('Close')
    },
  },
}
</script>

<style lang="scss" scoped>
.nav_links {
  position: absolute;
  bottom: 0;
  margin: 5vh 5vw;
  font-weight: 600;
  letter-spacing: 1px;
  ul {
    list-style: none;
    li {
      // font-size: 7.5rem;
      font-size: clamp(4rem, 10vw, 7.5rem);

      a {
        text-decoration: none;
        color: #fff;
      }
    }
  }
}
</style>
