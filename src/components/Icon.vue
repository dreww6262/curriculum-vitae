<template>
    <div class="imageContainer">
      <img :src="src" />
    </div>
</template>
<script setup lang="ts">
import { computed } from "vue"
    const props = defineProps(['imgName']);
    const src = computed(() => "src/assets/" + props.imgName)
</script>
<style scoped lang="scss">
  .imageContainer {
    max-width: 50px;
    max-height: 50px;
    border-radius: 5px;
    overflow: hidden;
    box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px, rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px, rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  }
  img {
    max-width: 100%;
    max-height: 100%;
    display: block;
  }
</style>