<script>
import Card from './components/Card.vue';
export default {
    name: 'App',
    components: {
        Card
    },
    data() {
        return {
            data: null,
            loading: false,
            error: null
        }
    },
    created() {
    this.fetchData();
  },
    methods: {
        async fetchData() {
            this.loading = true;
            try {
                const response = await fetch('https://fakestoreapi.com/products');
                if (!response.ok) {
                    throw new Error('Network response was not ok');
                }
                this.data = await response.json();
            } catch (error) {
                this.error = error;
            } finally {
                this.loading = false;
            }
        }
    },
}
</script>

<template>
<div class=" pt-6 py-6 bg-gray-50 font-inter">
    <h2 class="mx-15 text-2xl text-blue-900"><b>Our Team</b></h2>
    <p class=" mx-15 text-xl mt-2 text-gray-400">Worem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum, ac aliquet odio mattis.</p>

    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6 mx-15 my-10 ">
        <div v-if="loading">Loading...</div>
    <div v-else>
      <div v-for="product in data" :key="product.id">
        <Card :price="product.price" :title="product.title" :description="product.description" />
      </div>
    </div>
    </div>
</div>
</template>

<style>

</style>
