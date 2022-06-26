<script setup lang="ts">
import { ref } from 'vue'
import Icon from '../assets/faceless.svg'
defineProps<{ msg: string }>()

const count = ref(0)
</script>

<template>
<section class="main-content">
        <img :src="Icon" alt="" class="face-icon">
        <p class="face-title">Faceless Protocol</p>
        <div class="face-detail">A Cross-Platform Private Payment Scheme for Human-Readable Identifiers</div>
        <a class="wp-link" target="blank" href="https://docsend.com/view/9c7ubij47dk75sta">whitepaper</a>
</section>
</template>

<style scoped>
.main-content {
    height: calc(100vh - 52px);
    display: flex;
    color: #fff;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}

.face-icon {
    width: 300px;
}
.face-title {
    font-weight: 800;
    font-size: 20px;
}
.face-detail {
    margin-top: 24px;
    width: 370px;
    font-size: 18px;
}
.wp-link {
    margin-top: 24px;
    display: block;
    text-decoration: none;
    padding: 10px 26px;
    border: 1px solid #8a6de9;
    color: #8a6de9;
    border-radius: 6px;
    cursor: pointer;
}
.wp-link:hover {
    color: #007aff;
    border: 1px solid #007aff;
}

</style>
