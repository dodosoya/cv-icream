<<<<<<< HEAD
<script setup lang="ts">
const { t } = useI18n()
const router = useRouter()
</script>

<template>
  <div class="h-full flex flex-col justify-center items-center gap-10">
    <div class="text-6xl">
      {{ t('layout.title') }}
    </div>
    <div class="flex gap-10 text-lg">
      <button btn>
        {{ t('layout.button.upload_cv') }}
      </button>
      <button btn @click="router.push('template')">
        {{ t('layout.button.next_step') }}
      </button>
    </div>
  </div>
</template>

<route lang="yaml">
meta:
  layout: home
</route>
=======
<script setup lang="ts">
const { t } = useI18n()
const router = useRouter()
</script>

<template>
  <div class="h-full flex flex-col justify-center items-center gap-10">
    <div>{{ t('layout.title') }}</div>
    <div class="flex gap-10">
      <button btn>
        <div i-heroicons-outline-plus-sm class="icon inline-block align-text-bottom" />
        {{ t('layout.button.upload_cv') }}
      </button>
      <button btn @click="router.push('template')">
        <div i-heroicons-outline-arrow-circle-right class="icon inline-block align-text-bottom" />
        {{ t('layout.button.next_step') }}
      </button>
    </div>
  </div>
</template>

<route lang="yaml">
meta:
  layout: home
</route>
>>>>>>> develop
