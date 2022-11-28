<script>
import Child from "@/components/Child.vue";
export default {
  components: { Child },
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    incrementCount(i) {
      this.count += i;
      this.$root.hello();
    },
  },
};
</script>

<template>
  <!-- https://vuejs.org/guide/components/events.html#emitting-and-listening-to-events -->
  <Child v-on:add="incrementCount" />
  <p>Count: {{ count }}</p>
</template>
