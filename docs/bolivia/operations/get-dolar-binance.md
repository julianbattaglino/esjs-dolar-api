---
aside: false
outline: false
title: Dólar Binance
head:
  - [
    'meta',
    {
      name: 'description',
      content: 'API de cotizaciones de monedas extranjeras en Bolivia',
    },
  ]
  - [
    'meta',
    {
      name: 'keywords',
      content: 'bolivia, dolar, dolar api, dolar api bolivia',
    },
  ]
  - [
    'meta',
      {
        property: 'og:image',
        content: 'https://dolarapi.com/docs/assets/og.png',
      },
    ]
  - [
    'meta',
    {
      property: 'og:title',
      content: 'API para obtener el precio del Dólar en Chile',
    },
  ]
  - [
    'meta',
    {
      property: 'og:description',
      content: 'API de cotizaciones de monedas extranjeras en Chile',
    },
  ]
  - ['meta', { property: 'og:url', content: 'https://dolarapi.com' }]
  - ['meta', { property: 'og:site_name', content: 'DolarApi.com' }]
  - ['meta', { property: 'og:type', content: 'website' }]
  - ['meta', { property: 'og:locale', content: 'es_AR' }]
  - ['meta', { property: 'twitter:card', content: 'summary_large_image' }]
  - ['meta', { property: 'twitter:description', content: 'API de cotizaciones de monedas extranjeras en Chile' }]
  - ['meta', { property: 'twitter:title', content: 'API para obtener el precio del Dólar en Chile' }]
  - ['meta', { property: 'twitter:site', content: '@dolarapi' }]
  - ['meta', { property: 'twitter:creator', content: '@enzonotario_' }]
  - ['meta', { property: 'twitter:image', content: 'https://dolarapi.com/docs/assets/og.png' }]
  - ['meta', { property: 'twitter:url', content: 'https://dolarapi.com' }]
---

<script setup>
import { setRegionForSidebar } from '../../.vitepress/sidebar/sidebar.utils.js'

setRegionForSidebar('bo')
</script>

<OAOperation operationId="get-dolar-binance" :hide-default-footer="false">

<template #description="description">

<PathEndpoint :method="description.method" :path="description.path" :baseUrl="description.baseUrl" />

Cotización del dólar estadounidense en pesos bolivianos según Binance

</template>

<template #try-it="tryIt">

<TryItButton :operation-id="tryIt.operationId" :method="tryIt.method" hide-endpoint>

<template #response="response">

<OACodeBlock :code="JSON.stringify(response.response, null, 2)" lang="json" label="JSON" :is-dark="tryIt.isDark" :disable-html-transform="response.response.length > 1000" />
             
</template>

</TryItButton>

</template>

<template #footer>

<OAFooter />

<!--@include: ./parts/get-dolar-binance-footer.md -->

</template>

</OAOperation>
