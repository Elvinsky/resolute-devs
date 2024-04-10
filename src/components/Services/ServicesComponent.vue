<template>
  <div class="services">
    <h2 class="services__header">Our services</h2>
    <div class="services__content">
      <ServiceItem>
        <template #default><p>Copywriting</p></template>
        <template #icons>
          <FigmaIcon />
          <PhotoshopIcon />
          <IllustratorIcon />
        </template>
      </ServiceItem>
      <ServiceItem>
        <template #default><p>UI/UX Design</p></template>
        <template #icons>
          <FigmaIcon />
          <PhotoshopIcon />
          <IllustratorIcon />
        </template>
      </ServiceItem>
      <ServiceItem>
        <template #default> <p>Front-End Development</p> </template>
        <template #icons>
          <HTMLIcon />
          <CSSIcon />
          <JSIcon />
          <VueIcon />
        </template>
      </ServiceItem>
      <ServiceItem>
        <template #default> <p>Back-End Development</p> </template>
        <template #icons>
          <PythonIcon />
          <NodeIcon />
          <PHPIcon />
        </template>
      </ServiceItem>
      <ServiceItem>
        <template #default> <p>SEO Optimization</p> </template>
        <template #icons>
          <FigmaIcon />
          <PhotoshopIcon />
          <IllustratorIcon />
        </template>
      </ServiceItem>
      <ServiceItem>
        <template #default> <p>Deployment</p> </template>
        <template #icons>
          <FigmaIcon />
          <PhotoshopIcon />
          <IllustratorIcon />
        </template>
      </ServiceItem>
    </div>
  </div>
</template>

<script setup lang="ts">
import ServiceItem from '@/components/Services/ServiceItem.vue'
import FigmaIcon from '@/assets/icons/services/FigmaIcon.vue'
import IllustratorIcon from '@/assets/icons/services/IllustratorIcon.vue'
import PhotoshopIcon from '@/assets/icons/services/PhotoshopIcon.vue'
import HTMLIcon from '@/assets/icons/services/HTMLIcon.vue'
import CSSIcon from '@/assets/icons/services/CSSIcon.vue'
import JSIcon from '@/assets/icons/services/JSIcon.vue'
import VueIcon from '@/assets/icons/services/VueIcon.vue'
import NodeIcon from '@/assets/icons/services/NodeIcon.vue'
import PHPIcon from '@/assets/icons/services/PHPIcon.vue'
import PythonIcon from '@/assets/icons/services/PythonIcon.vue'
</script>

<style scoped lang="scss">
.services {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: var(--space-l);
  position: relative;
  z-index: 2;
  margin-top: var(--space-5xl);

  &__header {
    font-family: var(--font-roboto-bold);
    font-size: var(--font-size-h2-pc-tablet);
    color: var(--color-white-main);
    text-decoration: underline;
    text-underline-offset: 12px;
  }

  &__content {
    display: flex;
    flex-direction: column;
    gap: 8px;
    align-items: start;
    justify-content: start;
    width: 100%;
  }
}
</style>
