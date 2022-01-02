<template>
  <a href="#" @click="onClick">
    {{ text }}
  </a>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  props: {
    text: String,
    onClick: Function,
  },
})
export default class Button extends Vue {
  text!: string;
  onClick!: Function;
}
</script>

<style scoped lang="scss">
a {
  &:hover {
    text-decoration: unset;
  }
}
</style>