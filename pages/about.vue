<template>
  <div>
    <h2>About</h2>
    <p>
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. corrupti eos
      adipisci nam repellat possimus aperiam fugiat non? Laudantium, reiciendis
      repudiandae.
    </p>
    <p>
      Temporibus qui libero exercitationem repellendus, doloremque sit
      necessitatibus ab at
    </p>
    <div>
      {{ data }}
    </div>
  </div>
</template>

<script setup>
  const { data } = await useFetch("/api/currency/USD");
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
