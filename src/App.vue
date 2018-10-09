<template lang="pug">
  #app
    Usagi(knk)
    p(Usagi(knk)はきなこの写真がたくさん)
</template>

<script>
import Usagi from "@/components/Usagi.vue";

export default {
  name: "app",
  components: {
    Usagi
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #333;
  margin-top: 0px;
  border: solid 1px;
}
</style>
