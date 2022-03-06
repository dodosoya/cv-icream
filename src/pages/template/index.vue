<script setup lang="ts">
const { t } = useI18n()
const router = useRouter()
</script>

<template>
  <div class="h-full flex flex-col justify-center items-center gap-10">
    <div>{{ t('template.title') }}</div>
    <div class="flex gap-10">
      <button btn @click="router.back()">
        {{ t('template.button.back') }}
      </button>
      <button btn @click="router.push('edit')">
        {{ t('template.button.next_step') }}
      </button>
    </div>
  </div>
</template>

<route lang="yaml">
meta:
  layout: home
</route>
