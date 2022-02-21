<script setup lang="ts">
import ProductList from './components/ProductList.vue'
</script>

<template>
  <div class="App">
    <h1><span role="img" aria-label="Store emoji"> 🏪 </span> Good Store</h1>
    <ProductList />
  </div>
</template>

<style>
.App {
  font-family: sans-serif;
  text-align: center;
}

.ProductList {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 16px;
  justify-items: center;
  margin-top: 16px;
}

.ProductCard {
  /* Add shadows to create the "card" effect */
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.1);
  transition: 0.3s;
  border-radius: 8px;
  width: 200px;
}

.ProductCard img {
  width: 100%;
  height: 200px;
  object-fit: contain;
}

.ProductCard p {
  text-overflow: ellipsis;
  height: 50px;
  overflow: hidden;
}

/* On mouse-over, add a deeper shadow */
.ProductCard:hover {
  box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.1);
}

/* Add some padding inside the card container */
.ProductDescription {
  padding: 2px 16px;
}

.ProductSearch {
  padding: 8px;
  border-radius: 8px;
  border: none;
  border: 1px rgb(238, 238, 238) solid;
}
</style>
