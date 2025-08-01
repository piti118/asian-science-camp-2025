<template>
  <div>
    <vue-word-cloud v-bind="props" />
  </div>
</template>

<script>
import VueWordCloud from 'vuewordcloud';

export default {
  name: 'WordCloud',
  components: {
    VueWordCloud,
  },
  props: {
    // Define props to pass through to vuewordcloud
  },
  computed: {
    props() {
      return this.$props;
    },
  },
};
</script>

<style scoped>
/* Add any custom styles here */
</style>style