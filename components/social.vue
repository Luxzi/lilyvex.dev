<template>
  <NuxtLink :to="link">
    <Icon :name="icon" style="vertical-align: middle;" :alt="alt" :size="size"/>
  </NuxtLink>
</template>

<script lang="ts" setup>
  defineProps({
    alt: {
      type: String,
      required: true
    },
    icon: {
      type: String,
      default: ''
    },
    link: {
      type: String,
      default: ''
    },
    size: {
      type: String,
      default: '2em'
    },
  })
</script>

<style>

</style>