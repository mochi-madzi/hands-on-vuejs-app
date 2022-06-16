<template>
  <v-container>
    <v-row justify="center" align-content="center">
      <v-col>
        <div class="logo py-4 d-flex justify-center">
          <img
            class="vuetify-logo"
            alt="Vuetify Logo"
            src="/yumekawa_animal_hitsuji.png"
          />
        </div>
        <v-card-title class="text-h5 justify-center">
          Hello World
        </v-card-title>
      </v-col>
    </v-row>

    <v-row justify="center" align="center">
      <v-col
        cols="12"
        xs="12"
        sm="6"
        md="4"
        lg="3"
        v-for="item in items"
        :key="item.key"
      >
        <v-card>
          <v-img :aspect-ratio="1 / 1" :src="item.img"></v-img>

          <v-card-title>Cafe Badilico</v-card-title>

          <v-card-text>
            <p>
              Vuetify is a progressive Material Design component framework for
              Vue.js. It was designed to empower developers to create amazing
              applications.
            </p>
          </v-card-text>
          <v-card-actions>
            <v-spacer />
            <v-btn color="primary" nuxt to="/about"> Continue </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      items: [
        { img: "/food/sweets_ichigo_mousse.png" },
        { img: "/food/sweets_chagashi.png" },
        { img: "/food/sweets_momoji_manju.png" },
        { img: "/food/sweets_purin_cup.png" },
        { img: "/food/sweets_warabimochi_kuromitsu.png" },
        { img: "/food/sweets_tiramisu.png" },
      ],
    };
  },
};
</script>

<style scoped></style>
