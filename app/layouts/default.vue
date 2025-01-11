<script setup lang="ts">
  useHeadAndMeta()
  useOgImage()
</script>

<template>
  <div>
    <main>
      <DarkModeSwitch
        style="
          position: absolute;
          right: 0;
          z-index: 10;
          margin-top: 12px;
          margin-bottom: 12px;
        "
      />
      <slot />
    </main>
  </div>
</template>
<style></style>
