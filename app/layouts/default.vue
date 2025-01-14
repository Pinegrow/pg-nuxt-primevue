<script setup lang="ts">
  const route = useRoute()

  const pageMeta = computed(() => {
    return {
      title: route.meta.title,
      description: route.meta.description,
      ogImage: route.meta.ogImage,
      canonicalUrl: route.meta.canonicalUrl || route.fullPath,
      generator: route.meta.generator,
      tags: route.meta.tags,
    }
  })

  useHeadAndMeta(pageMeta)
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
