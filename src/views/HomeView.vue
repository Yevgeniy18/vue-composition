<template>
  <div class="home">
    <input type="text" placeholder="Enter something" v-model="query" />
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "HomeView",
  props: {},
  setup() {
    const query = ref<string>("");

    return {
      query,
    };
  },
});
</script>

<style lang="scss" scoped>
.home {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 80vh;
}

input {
  border-radius: 5px;
  outline: none;
  padding: 10px;
  font-size: 17px;
  width: 300px;
}
</style>
