<template>
  <router-link :to="to" aria-label="logo">
    <slot></slot>
  </router-link>
</template>

<script>
export default {
  props: {
    to: {
      required: false,
      type: string,
    },
  },
};
</script>
