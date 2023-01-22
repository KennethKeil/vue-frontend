<template>
  <v-card outlined>
    <v-card-title>{{ product.name }}</v-card-title>
    <v-card-subtitle>${{ product.price }}</v-card-subtitle>
    <v-card-actions>
      <v-btn @click="addToCart" color="success" outlined>
        Add to Cart
    </v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
  props: {
    product: Object,
    addToCart: Function
  }
}
</script>
