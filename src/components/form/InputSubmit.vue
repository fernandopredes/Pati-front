<template>
  <input type="submit" :value="text">
</template>

<script lang="ts">
import { defineComponent } from 'vue';

const MyComponent = defineComponent({
  props: {
    text: {
      type: String,
      default: "",
    },
  },
});

export default MyComponent

</script>

<style scoped>
input[type="submit"] {
  width: 200px;
  margin: 0 auto;
  text-transform: uppercase;
  color: #fff;
  background-color: #25282e;
  transition: .5s;
  border: 0;
  padding: 12px;
  cursor: pointer;
}
input[type="submit"]:hover {
  background-color: #141619;
}
</style>
