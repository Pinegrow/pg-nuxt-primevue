<script setup lang="ts">
  import siteMeta from '@/site'
  const { title, logo } = siteMeta
</script>
<template>
  <NuxtLink data-pg-name="Logo" class="flex items-center sm:flex-row" to="/">
    <BaseIcon height="40" class="mt-2" :name="logo" />
    <h6
      class="text-primary-600 dark:text-primary-200 font-extrabold font-serif ml-2 mt-4 text-2xl"
    >
      {{ title }}
    </h6>
  </NuxtLink>
</template>
<style scoped>
  .flex {
    display: flex;
  }
  .items-center {
    align-items: center;
  }
  @media (min-width: 640px) {
    .sm\:flex-row {
      flex-direction: row;
    }
  }
  .mt-2 {
    margin-top: 0.5rem /* 8px */;
  }
  .text-primary-600 {
    --tw-text-opacity: 1;
    color: rgb(180 100 48 / var(--tw-text-opacity));
  }
  :is(.dark .dark\:text-primary-200) {
    --tw-text-opacity: 1;
    color: rgb(229 191 170 / var(--tw-text-opacity));
  }
  .font-extrabold {
    font-weight: 800;
  }
  .font-serif {
    font-family: 'Sora', 'Sora fallback', sans-serif;
  }
  .ml-2 {
    margin-left: 0.5rem /* 8px */;
  }
  .mt-4 {
    margin-top: 1rem /* 16px */;
  }
  .text-2xl {
    font-size: 1.5rem /* 24px */;
    line-height: 2rem /* 32px */;
  }
</style>
