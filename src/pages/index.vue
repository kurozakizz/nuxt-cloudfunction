<template>
  <div>
    <h3>Dashboard</h3>
    <ul>
      <li v-for="fact in facts" :key="fact.text">
        {{ fact.text }}
      </li>
    </ul>
  </div>
</template>

<script>
import fetch from "isomorphic-fetch";

export default {
  name: "index",
  async asyncData() {
    const response = await fetch("https://nuxt-ssr.firebaseio.com/facts.json");
    const facts = await response.json();
    return { facts };
  }
};
</script>

