<template>
  <v-card outlined>
    <v-card-tite>{{ product.name }}</v-card-tite>
    <v-card-subtitle>${{ product.price }}</v-card-subtitle>
    <v-card-actions>
      <v-btn color="success" outlined>
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
