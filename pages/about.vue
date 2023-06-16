<template>
  <div>
    <h2>About</h2>
    <p>
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Pariatur
      corporis optio molestias nam placeat fuga nihil in aliquam commodi,
      eligendi, labore expedita? Molestias asperiores voluptatibus velit qui
      optio! Necessitatibus, eligendi!
    </p>
    <p>
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Pariatur
      corporis optio molestias nam placeat fuga nihil in aliquam commodi,
      eligendi, labore expedita? Molestias asperiores voluptatibus velit qui
      optio! Necessitatibus, eligendi!
      <div>{{ data }}</div>
    </p>
  </div>
</template>

<script setup>
const {data} = await useFetch('/api/currency/GBP')
// const { data } = await useFetch("/api/ninja?name=mario", {
//   method: 'post', 
//   body: {
//     age: 30
//   }
// });
</script>

<style scoped>
h2 {
  margin-bottom: 20px;
  font-size: 36px;
}

p {
  margin: 20px 0;
}
</style>
