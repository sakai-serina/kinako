<template lang="pug">
  #app
    Usagi(isActiveBorder="true" color="blue")
      template(slot="knk")
        p きなこかわいい一番かわいいうさぎ
    Usagi(color="red")
      template(slot="serina")
        p せりなはきなこの飼い主
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
}
.header{
  margin-top: 0px;
  border: solid 1px;
}
</style>
