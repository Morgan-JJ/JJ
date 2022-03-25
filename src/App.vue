<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          :src="require('./assets/seriouspic.jpg')"
          transition="scale-transition"
          width="40"
        />

        <span class="font-weight-medium">Jiang Junhui</span>
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://www.youtube.com/watch?v=dQw4w9WgXcQ?autoplay=1"
        target="_blank"
        text
      >
        <span class="mr-2">Hehe</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <PageHeader />
      <accordion-body />
    </v-main>
  </v-app>
</template>

<script>
import AccordionBody from "./components/AccordionBody.vue";
import PageHeader from "./components/PageHeader";

export default {
  name: "App",

  components: {
    PageHeader,
    AccordionBody,
  },

  data: () => ({
    //
  }),
};
</script>
