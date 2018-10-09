<template lang="pug">
  .content(:class="borderClass")
    p うさぎ世界一番付
    slot(name="knk")
    slot(name="serina")
</template>

<script>
export default {
  name: "Usagi",
  props: {
    knk: String,
    isActiveBorder: Boolean,
    color: String,
  },
  computed: { //関数を定義
    borderClass() {
      return {
        border : this.isActiveBorder,
        red: this.color === 'red',
        blue: this.color === 'blue',
      }
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.border {
  margin-top: 0px;
  border: solid 1px;
}
.red {
  color: pink;
}
.blue {
  color: blue;
}
</style>
