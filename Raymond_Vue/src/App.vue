<script>
import Products from "./components/Products.vue";
import Header from './components/Header.vue';

export default {
  components: {
    Products,
    Header,
  },
};
</script>

<template>
  <div style="color: #3366cc; font-size: 20px;  padding-top: 56px;">
    <h1>Top Locations</h1>
    <Products />
    <Header/>
  </div>
</template>