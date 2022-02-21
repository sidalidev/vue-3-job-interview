<script setup lang="ts">
// Use me 🥺
import ProductCard from './ProductCard.vue'
import { getAllProducts } from '../api/products.api'

/**
 * As a User:
 *
 * 1. I see a list of the store's Products
 * 2. I can filter the listed Products
 * 3. (Bonus) I can sort them by Name(ascendant and descendant)
 */
</script>

<template>
  <div>
    <input class="ProductSearch" placeholder="Seach here..." />

    <div class="ProductList">
      <ProductCard
        :product="{
          id: 99,
          title: 'Fjallraven - Foldsack No. 1 Backpack, Fits 15 Laptops',
          price: 109.95,
          description:
            'Your perfect pack for everyday use and walks in the forest. Stash your laptop (up to 15 inches) in the padded sleeve, your everyday',
          image: 'https://fakestoreapi.com/img/81fPKd-2AYL._AC_SL1500_.jpg',
        }"
      />
    </div>
  </div>
</template>
