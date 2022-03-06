<template>
  <main class="h-full">
    <Header />
    <div class="content sm:flex sm:flex-row">
      <Toolbar class="sm:w-24" />
      <CVPreview class="text-center bg-white sm:flex-1 sm:border sm:border-t-0 border-gray-400" />
      <Sidebar class="sm:w-96" />
    </div>
    <router-view />
  </main>
</template>

<style scoped>
.content {
  height: calc(100% - 80px)
}
</style>
