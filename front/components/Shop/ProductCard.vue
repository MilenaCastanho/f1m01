<template>
    <div class="productContainer">
        <img :src="product.image" alt="product thumb" class="thumb">
        <div class="productInfo">
            <h4 class="productName">{{ product.name }}</h4>
            <p class="productDescription">{{ product.description }}</p>
            <p class="productPrice">{{ product.price }}</p>
            <p class="productCategory">{{ product.category }}</p>
            <p class="productStock">{{ product.stock }}</p>
            <p class="productRating">{{ product.rating }}</p>
            <NuxtLink :to="`/product/${product.id}`">
                <p class="viewP">View Detail</p>
            </NuxtLink>
        </div>
            <div class="productButtons">
                <!-- <button class="addToCart" @click="addToCart(product)">
                    <span>Add to Cart</span>
                </button>
                <button class="addToWishlist " @click="addToWishlist(product)">
                    <span>Add to Wishlist</span>
                </button> -->
            </div>
        </div>
</template>

<script setup lang="ts">

const { product } = defineProps(['product'])

</script>

<style scoped>
.productContainer {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    width: 100%;
    height: 100%;
    padding: 10px;
    background: #fff;
    border-radius: 5px;
    box-shadow: 1px 1px 10px rgba(231, 11, 11, 0.91);

</style>