<template>
  <nav>
    <ul>
      <li v-for="(item, index) in items" :key="index">
        {{ item }}
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  props: {
    items: {
      required: false,
      type: Array,
    },
  },
};
</script>


