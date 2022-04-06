<template>
  <mt-header fixed :title="title">
  </mt-header>
</template>
<script>
  import banner from "./banner";
export default {
  name: 'header',
  props: {
    title: String,
  },
  data() {
    return {};
  },
  computed: {},
  watch: {},
  components:{
    banner
  }
};

</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.mint-header {
  background-color: #2489eb;
  font-size: 1rem;
  height: 2.5rem;
}
</style>
