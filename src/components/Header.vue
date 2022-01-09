<template>
  <header>
    <navigation></navigation>
    <logo></logo>
    <navigation></navigation>
  </header>
</template>

<script>
import Logo from "./Logo.vue";
import Navigation from "./Navigation.vue";

export default {
  components: {
    Logo,
    Navigation,
  },
  props: {
    title: {
      required: false,
      type: String,
    },
  },
};
</script>