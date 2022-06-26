<script setup lang="ts">
defineProps<{ isError: Boolean, default: false }>()
</script>

<template>
    <div 
        v-if="!isError"
        class="unequal-container"
    >
        <div class="check-style-unequal-width"></div>
    </div>
    <div 
        v-else
        class='unequal-container error-check'
    >
        x
    </div>
</template>

<style scoped>
  .unequal-container {
        width: 20px;
        height: 20px;
        background: #00ffff;
        position: relative;
        left: 50%;
        transform: translate(-50%, 0);
        border-radius: 2px;
    }
    .error-check {
        background: rgba(0,255,255, 0.5);
        color: #000;
        text-align: center;
        font-weight: 900;
        line-height: 20px;
        font-size: 20px;
    }
    .check-style-unequal-width {
        width: 7px;
        height: 12px;
        border-color: #000;
        border-style: solid;
        border-width: 0px 3px 3px 0;
        transform: rotate(45deg);
        position: relative;
        left: 7px;
        top: 3px
    }
</style>
