<script setup lang="ts">
const link = () => {
    window.open('https://docsend.com/view/9c7ubij47dk75sta')
}
</script>

<template>
 <header class="header">
    <div class="main-icon">
        Faceless
    </div>
    <div class="left-box">
        <div class="router-btn active-route">Home</div>
        <div class="router-btn" @click="link">Docs</div>
    </div>
 </header>
</template>

<style scoped>
.header {
    display: flex;
    width: 100%;
    height: 52px;
    line-height: 52px;
    background: #000;
    padding: 0 40px;
    box-sizing: border-box;
}
.main-icon {
    height: 100%;
    font-weight: 800;
    font-size: 20px;
    line-height: 52px;
    color: #fff;
}
.left-box {
    height: 100%;
    margin-left: auto;
    display: flex;
}
.router-btn {
    height: 100%;
    padding: 0 16px;
    cursor: pointer;
    color: #fff;
}
.active-route, .router-btn:hover {
    background: linear-gradient(0deg, rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.1)),#0F4270;
    box-shadow: 0px 4px 4px 2px rgb(43 122 254 / 10%);
}
</style>
