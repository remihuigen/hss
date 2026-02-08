<script setup>
useHead({
  meta: [
    { name: 'viewport', content: 'width=device-width, initial-scale=1' }
  ],
  link: [
    { rel: 'icon', href: '/favicon.ico' }
  ],
  htmlAttrs: {
    lang: 'en'
  }
})

const title = 'Geen gezeik, geen HSS - Hoogspanninghoogverraad.nl'
const description = 'Boze burgers aller lande, verenigt u. Soest staat op tegen de komst van het hoogspanningsstation van Stedin. Sluit je aan bij de strijd tegen onrecht  .'

useSeoMeta({
  title,
  description,
  ogTitle: title,
  ogDescription: description,
  ogImage: '/naald.jpg',
  twitterImage: '/naald.jpg',
  twitterCard: 'summary_large_image'
})
</script>

<template>
  <UApp>
    <UHeader :ui="{toggle: 'hidden'}">
      <template #left>
        <NuxtLink to="/">
          <AppLogo class="min-w-20 max-w-36 shrink-0" />
        </NuxtLink>
      </template>

      <template #right>
        <p class="text-xs sm:text-sm text-muted">
          GEEN GEZEIK, GEEN HSS
        </p>
      </template>
    </UHeader>

    <UMain>
      <NuxtPage />
    </UMain>

    <USeparator icon="bi:emoji-angry-fill" />

    <UFooter>
      <template #left>
        <p class="text-sm text-muted">
          GEEN GEZEIK, GEEN HSS • © {{ new Date().getFullYear() }}
        </p>
      </template>

      <template #right>
       <p class="text-sm text-muted">
         HOOGSPANNINGHOOGVERRAAD.NL
        </p>
      </template>
    </UFooter>
  </UApp>
</template>
