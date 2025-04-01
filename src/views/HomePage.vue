<template>
  <div class="min-n-screen">
    <Suspense>
      <template #default>
        <div>
          <LoadingSpinner />
        </div>
      </template>
      <template #fallback>
        <div class="flex justify-center items-center min-h-screen">
          <LoadingSpinner />
        </div>
      </template>
    </Suspense>
  </div>
</template>

<script setup>
import LoadingSpinner from "@/components/LoadingSpinner.vue";
</script>
