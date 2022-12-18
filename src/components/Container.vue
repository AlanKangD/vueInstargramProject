<template>
  <div v-for="(a, i) in data" :key="i">
    <POST :a="a"/>
  </div>
</template>

<script>
import POST from './Post.vue';

export default {
    name : 'Container',
    components: {
      POST : POST,
  },
  props : {
    data : Array,
  }

}
</script>

<style>

</style>