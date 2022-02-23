<script setup lang="ts">
import type { ProductT } from '@/types'

defineProps<{
  product: ProductT
}>()
</script>

<template>
  <div class="ProductCard">
    <img :src="product.image" alt="{description}" />
    <div class="ProductDescription">
      <h4>{{ product.title }}</h4>
      <h3>{{ product.price }}€</h3>
      <p>{{ product.description }}</p>
    </div>
  </div>
</template>
