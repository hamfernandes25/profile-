<template>
  <header>
    <v-layout>
      <!-- <v-system-bar color="deep-purple darken-3"></v-system-bar> -->

      <v-app-bar color="primary" prominent>
        <v-app-bar-nav-icon
          variant="text"
          @click.stop="drawer = !drawer"
        ></v-app-bar-nav-icon>

        <v-toolbar-title>Resume</v-toolbar-title>

        <v-spacer></v-spacer>
      </v-app-bar>

      <v-navigation-drawer v-model="drawer" location="top" temporary>
        <v-list><a href="#">Profile</a></v-list>
        <v-list><a href="#">Qualifications</a></v-list>
        <v-list><a href="#">Projects</a></v-list>
      </v-navigation-drawer>
    </v-layout>
  </header>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
//import CardView from './card.vue'

export default {
  name: "HeaderView",
  components: {
    // HelloWorld,
    // CardView,
  },
  data: () => ({
    drawer: false,
    group: null,
    items: [
      {
        title: "Foo",
        value: "#",
      },
      {
        title: "Bar",
        value: "bar",
      },
      {
        title: "Fizz",
        value: "fizz",
      },
      {
        title: "Buzz",
        value: "buzz",
      },
    ],
  }),

  watch: {
    group() {
      this.drawer = false;
    },
  },
};
</script>
