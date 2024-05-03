<template>
    <div>
      <h1>Experience</h1>
      <div v-for="(item, index) in value" :key="index">
        <div class="item-card">
          <h2>{{ item.title }}</h2>
          <p>{{ item.description }}</p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      value: {
        type: Array,
        required: true
      }
    }
  };
  </script>
  
  <style scoped>
  .item-card {
    border: 1px solid #ccc;
    padding: 10px;
    margin-bottom: 10px;
  }
  </style>
  