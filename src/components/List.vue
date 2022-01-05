<template>
  <ul>
    <li v-for="item in items" :key="item.id">
      {{ item.message }}
    </li>
  </ul>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  props: {
    items: Array,
  },
})
export default class Button extends Vue {
  text!: Array<Object>;
}
</script>

<style scoped lang="scss">
ul {
  list-style-type: none;
}
</style>