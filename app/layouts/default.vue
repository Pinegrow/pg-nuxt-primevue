<script setup lang="ts">
  useHeadAndMeta()
  useOgImage()
</script>

<template>
  <div>
    <main>
      <slot />
    </main>
  </div>
</template>
<style>
  @import '~/assets/css/global.css';
  @import '~/assets/css/main.css';
</style>
