<template>
  <div class="min-n-screen">
    <Suspense>
      <template #default>
        <div class="font-playfair">
          <NavBar />
          <HeroSection />
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
import NavBar from "@/components/NavBar.vue";
import HeroSection from "@/components/HeroSection.vue";
</script>
