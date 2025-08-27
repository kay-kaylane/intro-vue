<script setup>
const props = defineProps({
    title: String,
    price: Number,
    image: String,
    inStock: Boolean
})
</script>

<template>
    <div class="card" v-if="title">
        <img v-if="image" :src="image" :alt="title" class="product-image" />
        <h3>{{ title }}</h3>
        <p>Preço: R$ {{ price}}</p>
        <div :class="inStock ? 'ativo' : 'inativo'">
            {{ inStock ? 'Em estoque' : 'Fora de estoque' }}
        </div>
    </div>
</template>

<style scoped>
.card {
    border: 1px solid #ccc;
    padding: 1rem;
    margin: 1rem;
    width: 220px;
    text-align: center;
}
.product-image {
    width: 180px;
    height: 180px;
    object-fit: cover;
    margin-bottom: 0.5rem;
}
.ativo {
    color: green;
    font-weight: bold;
}
.inativo {
    color: red;
    font-weight: bold;
}
</style>