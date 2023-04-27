<template>
  <div>Index</div>
  <Link href="/hello">Show Page</Link>
  <div>The message is {{ message }}</div>
</template>

<script setup lang="ts">
import { Link } from '@inertiajs/vue3'

export interface Props {
  message?: string
}

withDefaults(defineProps<Props>(), {
  message: ''
})
</script>

<style lang="scss" scoped></style>
