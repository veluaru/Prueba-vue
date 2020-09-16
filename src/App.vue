<template>
  <v-app>
    <v-app-bar
      color="indigo darken-2"
      dark
      shrink-on-scroll
      scroll-target="#scrolling-techniques"
      class="shrink"
    >
      <v-toolbar-title>Mi Galeria de Imágenes</v-toolbar-title>
    </v-app-bar>
    <v-main>
      <HelloWorld v-bind:images="images" />
      <ImageList />
    </v-main>
  </v-app>
</template>

<script>
import ImageList from "./components/ImageList";
import HelloWorld from "./components/HelloWorld";
//import axios from "axios";

export default {
  name: "App",

  components: {
    HelloWorld,
    ImageList,
  },
  data() {
    return {
      images: [
        {
          id: 1,
          text: "mmmmm",
        },
        {
          id: 2,
          text: "asd",
        },
      ],
    };
  },
  // methods: {
  // beforeCreate() {
  //   console.log("holi");
  //   axios
  //     .get("https://api.coindesk.com/v1/bpi/currentprice.json")
  //     .then((response) => (this.images = response))
  //     .catch((err) => console.log(err));
  // },
  // },
};
</script>
