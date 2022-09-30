<template>
  <div class="defaultWrapper">
    <Theheader />
    <nuxt />
    <Thefooter />
  </div>
</template>

<script>
import Theheader from "../components/Theheader.vue";
import Thefooter from "../components/Thefooter.vue";
export default {
  components: { Theheader, Thefooter },
};
</script>

<style lang="scss">
.defaultWrapper {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
</style>