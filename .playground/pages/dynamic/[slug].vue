<template>
  <div>
    <pre>
      {{ $route?.params }}
    </pre>
  </div>
</template>


<script setup>

import { useRoute, defineOgImage,defineOgImageComponent, definePageMeta, useServerSeoMeta } from '#imports'

let route = useRoute();

defineOgImageComponent('Nuxt', {
  headline: route?.params?.slug,
  title: 'Version 3 🎉',
  description: 'Nuxt OG Image v3 is here!',
})
</script>
