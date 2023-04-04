<script setup lang="ts">
const name = "Andrew Williamson"
const blurb = "Creating Full Stack Web Based Solutions Since 2020"
</script>

<template>
    <div class="align-center">
        <img alt="Vue logo" class="logo" src="@/assets/logo.png" width="125" height="125" />
        <h2>{{ name }}</h2>
        <h4>{{ blurb }}</h4>
    </div>
</template>

<style scoped lang="scss">
.align-center {
    display: flex;
    flex-direction: column;
    align-items: center;
}
.logo {
    padding-bottom: 8px;
}
</style>