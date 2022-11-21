<template>
  <div class="greetings">
    <h1 class="green">An example of an emit: </h1>
  </div>
</template> 

<style scoped>
h1 {
  font-weight: 400;
  font-size: 2rem;
  top: -10px;
}

.greetings h1 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
