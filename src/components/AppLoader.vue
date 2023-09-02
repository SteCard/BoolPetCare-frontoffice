<!-- JAVASCRIPT & VUE.JS -->
<script>
export default {
}
</script>

<!-- TEMPLATE HTML -->
<template lang="">
    <div class="loader"></div>
</template>

<!-- STYLE SCSS -->
<style lang="scss">

@use '../styles/generals.scss' as *;

.loader {
    border: 15px solid #f3f3f3;
    border-top: 15px solid #3498db;
    border-radius: 50%;
    width: 100px;
    height: 100px;
    animation: spin 2s linear infinite;
}
@keyframes spin {
    0% {
        transform: rotate(0deg);
    }
    100% {
        transform: rotate(360deg);
    }
}
</style>