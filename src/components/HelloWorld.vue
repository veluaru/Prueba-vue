<template>
  <v-container>
    <h1>Esto funciona</h1>
    <imagelist />
  </v-container>
</template>

<script>
import imagelist from "./ImageList";

export default {
  name: "HelloWorld",
  components: {
    imagelist,
  },

  data: () => ({}),
};
</script>
