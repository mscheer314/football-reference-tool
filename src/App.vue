<template>
  <p>This is my page.</p>
</template>

<script lang="ts">
import axios from "axios";

import { defineComponent } from "vue";

export default defineComponent({
  name: "App",
  components: {},
  methods: {
    callBackendTest: () => {
      axios.get("/home").then(console.log("I made it back."));
    },
  },
});
</script>

<style></style>
