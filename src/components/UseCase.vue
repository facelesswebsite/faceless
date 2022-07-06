<script setup lang="ts">
import { ref } from 'vue'
import Icon1 from '../assets/icon1.svg'
import Icon2 from '../assets/icon2.svg'
import Icon3 from '../assets/icon3.svg'
import Icon9 from '../assets/127711656246680_.pic.jpg'
defineProps<{ msg: string }>()

const count = ref(0)
</script>

<template>
<section class="use-case">
        <div class="title-wrapper">
            <div class="title">Use Cases</div>
        </div>
        <div class="content-wrapper">
            <div class="content-item">
                <div class="image" style="border-radius: 10px">
                    <img :src="Icon9" alt="">
                </div>
                <div class="content">
                    <div class="content-title">Electronic invoicing</div>
                    <p>is a natural application of our protocol given the fact that our payment is based on HRIs, the authenticity of which have been verified by our platforms.</p>
                </div>
            </div>
            <div class="content-item">
                <div class="image">
                    <img :src="Icon1" alt="">
                </div>
                <div class="content">
                    <div class="content-title">Regulation-compliant private payment</div>
                    <p>can be built on our system since our system is closely tied to the users’ HRIs,such as mobile numbers and social media accounts.</p>
                </div>
            </div>
            <div class="content-item">
                 <div class="image">
                    <img :src="Icon2" alt="">
                </div>
                <div class="content">
                    <div class="content-title">Trust-based DeFi systems</div>
                    <p>such as credit systems, lending, etc can be built on privacy-preserving analysis of various information across different payment and social media platforms, etc.</p>
                </div>
            </div>
            <div class="content-item">
                <div class="image">
                    <img :src="Icon3" alt="">
                </div>
                <div class="content">
                    <div class="content-title">Financial management for a hierarchical organization</div>
                    <p>it can be built on top of extensions of IBE, such as hierarchical IBE, which allows a key holder for “company.eth” to decrypt the ciphertext for “department.company.eth”.</p>
                </div>
            </div>
        </div>
</section>
</template>

<style scoped>
    .use-case{
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
        margin-top: 80px;
    }
    .content-item{
        padding: 30px 0;
        display: flex;
        align-items: center;
    }
    .content-title{
        margin-bottom: 24px;
        font-size: 22px;
    }
    .content p{
        margin-bottom: 8px;
        font-size: 16px;
        color: #ccc;
    }
    .image{
        height: 160px;
        width: 160px;
        padding: 30px;
    }
    .image img {
        width: 100px;
        height: 100px;
        border-radius: 50px;
    }
</style>
