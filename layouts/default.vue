<template>
  <v-app dark>
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
    }
  },
}
</script>

<style lang="scss" scoped></style>
