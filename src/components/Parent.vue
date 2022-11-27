<script>
  import Child from "@/components/Child.vue";
  export default {
    components: {Child},
    data() {
      return {
        count: 0
      }
    }
  }
</script>

<template>
  <!-- https://vuejs.org/guide/components/events.html#emitting-and-listening-to-events -->
  <Child v-on:add="(i) => count += i" />
  <p>Count: {{ count }}</p>
</template>
