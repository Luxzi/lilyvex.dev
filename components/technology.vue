<template>
  <NuxtLink :to="link">
    <Icon :name="icon" style="vertical-align: middle;"/> <p>{{ label }}</p>
  </NuxtLink>
</template>

<script lang="ts" setup>
  defineProps({
    label: {
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
    }
  })
</script>

<style scoped>
  p {
    display: inline;
    text-decoration: underline;
    text-decoration-thickness: .05em;
  }
</style>