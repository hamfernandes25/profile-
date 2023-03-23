<template>
  <div class="bg-teal d-flex w-100 align-center px-4">
    <strong>Get connected with me on social networks!</strong>

    <v-spacer></v-spacer>

    <v-btn
      v-for="icon in icons"
      :key="icon"
      class="mx-4"
      :icon="icon"
      variant="plain"
      size="small"
    ></v-btn>
  </div>

  <div class="px-4 py-2 bg-black text-center w-100">
    @{{ new Date().getFullYear() }}
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
//import CardView from './card.vue'

export default {
  name: "FooterView",
  components: {
    // HelloWorld,
    // CardView,
  },
  data: () => ({
    icons: ["mdi-facebook", "mdi-twitter", "mdi-linkedin", "mdi-instagram"],
  }),
};
</script>
