<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <h1 class="text-3xl font-bold underline">
    {{ msg }}
  </h1>

  <div class="card grid gap-4">
    <button type="button" class="bg-primary-500" @click="count++">
      count is {{ count }}
    </button>
    <button type="button" class="bg-neutral">
      Learn more
    </button>
  </div>
</template>
