<template>
  <div>
    <v-row
      v-for="product in $store.state.products"
      :key="product.name"
    >
      <HorizontalProduct
        :product="product"
        btnAction="remove"
       />
    </v-row>
  </div>
</template>

<script>
import { mapState } from 'vuex'
import HorizontalProduct from '@/components/cards/HorizontalProduct.vue'

export default {
  components: {
    HorizontalProduct
  },
  data() {
    return {}
  },
  computed: {
    ...mapState(['products'])
  },
  methods: {
    removeFromCart() {
    }
  }
}
</script>
