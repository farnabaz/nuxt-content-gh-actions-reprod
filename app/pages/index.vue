<script setup lang="ts">
const siteConfig = useAsyncData('site-config', async () => queryCollection('siteConfig').first())
</script>
<template>
  index page
  <pre>
    {{ siteConfig.data.value }}
  </pre>
</template>
