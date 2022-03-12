<script setup lang="ts">
const { t } = useI18n()
const router = useRouter()
</script>

<template>
  <div class="h-full flex flex-col justify-center items-center gap-10 ">
    <div class="text-6xl text-center">
      {{ t('home.title') }}
    </div>
    <div>
      <button btn text-lg @click="router.push('layout')">
        {{ t('home.button.start_cv') }}
      </button>
    </div>
  </div>
</template>

<route lang="yaml">
meta:
  layout: home
</route>
