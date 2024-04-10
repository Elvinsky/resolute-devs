<template>
  <section class="page">
    <HeaderComponent />
    <div class="content">
      <BackgroundCircle />
      <IntroComponent />
      <ServicesComponent />
      <BenefitsComponent />
    </div>
  </section>
</template>

<script setup lang="ts">
import HeaderComponent from '@/components/Header/HeaderComponent.vue'
import IntroComponent from '@/components/WebIntro/IntroComponent.vue'
import BackgroundCircle from '@/components/BackgroundCircle/BackgroundCircle.vue'
import ServicesComponent from '@/components/Services/ServicesComponent.vue'
import BenefitsComponent from '@/components/Benefits/BenefitsComponent.vue'
</script>

<style scoped lang="scss">
.page {
  padding: var(--space-safe);
  background-color: var(--color-black-main);
  height: 100%;
}

.content {
  width: 80%;
  margin: auto;
  color: white;
  display: flex;
  flex-direction: column;
}
</style>
