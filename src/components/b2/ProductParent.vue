<template>
  <div>
    <ProductChildren :product="product"></ProductChildren>
  </div>
</template>

<script setup>
import ProductChildren from "@/components/b2/ProductChildren.vue";

const product = {
  id: 1,
  productName: "Bưởi ba Roi",
  price: 12000,
  quantity: 10,
};
</script>

<style></style>
