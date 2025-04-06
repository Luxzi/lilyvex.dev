<template>
  <Button @click="copyToClipboard" class="cursor-pointer">Copy to clipboard <Icon :name="icon" style="vertical-align: middle;" :alt="name" size="1.5em" /></Button>   
</template>

<script lang="ts" setup>
const props = defineProps<{
  name: string,
  icon?: string,
  address?: string
}>()

const copyToClipboard = () => {
  const text = props.address
  if (text) {
    navigator.clipboard.writeText(text)
      .then(() => {
        alert('Copied! ✨')
      })
      .catch(err => {
        console.error('Copy failed', err)
      })
  }
}
</script>

<style scoped>
Button {
  font-family: "Kode Mono", monospace;
}
</style>