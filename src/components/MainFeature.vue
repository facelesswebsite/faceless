<script setup lang="ts">
import { ref } from 'vue'
import Icon4 from '../assets/icon4.svg'
import Icon5 from '../assets/icon5.svg'
import Icon6 from '../assets/icon6.svg'
defineProps<{ msg: string }>()

const count = ref(0)
</script>

<template>
<section class="main-feature">
        <div class="title-wrapper">
            <div class="title">Main Feature</div>
        </div>
        <div class="content-wrapper">
            <div class="content-item">
                <div class="content-header">
                    <span class="title">HRI Anonymity & Amount confidentiality</span>
                    <img class="image" :src="Icon4" alt="">
                </div>
                <p class="content">
                    guarantee the user privacy, including the HRI anonymity and amount confidentiality.
                </p>
            </div>
            <div class="content-item">
                <div class="content-header">
                    <span class="title">One key to rule them all</span>
                    <img class="image" :src="Icon4" alt="">
                </div>
                <p class="content">
                    one secret key for managing multiple HRIs since each user could have many HRIs.
                </p>
            </div>
            <div class="content-item">
                <div class="content-header">
                    <span class="title">Privacy-preserving verification of HRIs</span>
                    <img class="image" :src="Icon4" alt="">
                </div>
                <p class="content">
                    prove you are who you claim you are.
                </p>
            </div>
        </div>
</section>
</template>

<style scoped>
    .main-feature{
        height: 100vh;
        color: #fff;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
    .title-wrapper{
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    
    .title{
        font-size: 32px;
    }
    .subtitle{
        margin-top: 16px;
        font-size: 24px;
        color: #ccc;
    }
    .content-wrapper{
        display: flex;
        justify-content: space-between;
        margin-top: 80px;
    }
    .content-item{
        padding: 48px 16px;
        border-radius: 8px;
        background: #14141A;
        width: 380px;
        transition: all ease .5s;
    }
    .content-item:hover{
        transform: scale(1.05);
    }
    .content-header{
        height: 130px;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
    .content-header .title{
        font-size: 22px;
    }
    .content{
        margin-bottom: 8px;
        font-size: 16px;
        line-height: 24px;
        color: #ccc;
        hyphens: auto;
    }
    .image{
        height: 130px;
        position: relative;
        left: 20px;
    }
</style>
