<script setup lang="ts">
import { ref } from 'vue'
import Icon7 from '../assets/127611656224842_.pic_hd.jpg'
import Qredo from '../assets/qredo-favicon-v2.png'
import METEMASK  from '../assets/metamask.jpg'
import Faceless from '../assets/faceless.svg'
import TorNado from '../assets/tornado.jpg'
import ENSICON from '../assets/ENs.jpg'
import StatusIcon from './StatusIcon.vue'

const count = ref(0)
</script>

<template>
<section class="compare">
        <div class="title-wrapper">
            <div class="title">Our solution compared with Existing Private Payment Solutions</div>
        </div>
        <div class="content-wrapper">
            <!-- <img class="image" :src="Icon7" alt=""> -->
            <table border="1" class="compare-table">
                <tr>
                    <th></th>
                    <th>
                        
                         <div class="table-title-item">
                            <img :src="METEMASK" alt="" class="table-title-icon">
                            METEMASK
                        </div>
                    </th>
                    <th>
                        <div class="table-title-item">
                            <img :src="Qredo" alt="" class="table-title-icon">
                            Qredo
                        </div>
                    </th>
                    <th>
                        <div class="table-title-item">
                            <img :src="TorNado" alt="" class="table-title-icon">
                            Tornado
                        </div>
                    </th>
                    <th>
                        <div class="table-title-item">
                            <img :src="ENSICON" alt="" class="table-title-icon">
                            ENS
                        </div>
                    </th>
                    <th>
                        <div class="table-title-item">
                            <img :src="Faceless" alt="" class="table-title-icon">
                            Faceless
                        </div>
                    </th>
                </tr>
                <tr>
                    <td>HRI-Compatible</td>
                    <td>
                        <StatusIcon :isError="true" />
                    </td>
                    <td>
                        <StatusIcon :isError="true" />
                    </td>
                    <td>
                        <StatusIcon :isError="true" />
                    </td>
                    <td><StatusIcon /></td>
                    <td><StatusIcon /></td>
                </tr>
                <tr>
                    <td>Regulation Compliant</td>
                    <td><StatusIcon /></td>
                    <td><StatusIcon /></td>
                    <td><StatusIcon :isError="true" /></td>
                    <td><StatusIcon :isError="true" /></td>
                    <td><StatusIcon /></td>
                </tr>
                <tr>
                    <td>Privacy Centric</td>
                    <td><StatusIcon :isError="true" /></td>
                    <td><StatusIcon :isError="true" /></td>
                    <td><StatusIcon /></td>
                    <td><StatusIcon :isError="true" /></td>
                    <td><StatusIcon /></td>
                </tr>
                <tr>
                    <td>Peak FDV</td>
                    <td>$7B</td>
                    <td>$20B</td>
                    <td>$4B</td>
                    <td>$8.5B</td>
                    <td>$20M</td>
                </tr>
            </table>
        </div>
</section>
</template>

<style scoped>
    .compare{
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
    .image{
        width: 1200px;
    }
    .compare-table {
        width: 100%;
        border-collapse: collapse;
    }
    .compare-table td,  .compare-table th{
        padding: 12px 18px;
        text-align: center;
    }
  
    .table-title-item {
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .table-title-icon {
        height: 22px;
        margin-right: 4px;
    }
  
</style>
