<template>
  <div class="benefits">
    <h2 class="benefits__header">Benefits</h2>
    <div class="benefits__content">
      <BenefitsItem>
        <template #header>Cutting-Edge Design</template>
        <template #content>
          Our team of skilled designers and developers work hand-in-hand to craft visually stunning
          and user-friendly websites. We stay ahead of the latest trends to ensure your website
          stands out.
        </template>
      </BenefitsItem>
      <BenefitsItem>
        <template #header>Customized Solutions</template>
        <template #content>
          We understand that every business is unique. That's why we offer tailored solutions to
          meet your specific needs, ensuring your website reflects the essence of your brand.
        </template>
      </BenefitsItem>
      <BenefitsItem>
        <template #header>Results-Driven Approach</template>
        <template #content>
          Our goal is to not just launch websites, but to create platforms that drive growth. From
          responsive design to SEO optimization.
        </template>
      </BenefitsItem>
      <BenefitsItem>
        <template #header>Seamless User Experience</template>
        <template #content>
          We prioritize usability in every project. By focusing on intuitive navigation and fast
          load times, we ensure a smooth experience for all your visitors.
        </template>
      </BenefitsItem>
      <BenefitsItem>
        <template #header>Ongoing Support</template>
        <template #content>
          Launching your website is just the beginning. We provide ongoing maintenance and support
          to keep your site up-to-date and performing at its best.
        </template>
      </BenefitsItem>
      <BenefitsItem>
        <template #header>Proffesional team</template>
        <template #content>
          Our team is dedicated to upholding the highest standards of quality in every project we
          undertake. From meticulous planning to rigorous testing.
        </template>
      </BenefitsItem>
    </div>
  </div>
</template>

<script setup lang="ts">
import BenefitsItem from './BenfitsItem.vue'
</script>

<style scoped lang="scss">
.benefits {
  margin-top: var(--space-5xl);
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: var(--space-xl);
  position: relative;
  z-index: 2;

  &__header {
    font-family: var(--font-roboto-bold);
    font-size: var(--font-size-h2-pc-tablet);
    color: var(--color-white-main);
    text-decoration: underline;
    text-underline-offset: 12px;
    align-self: self-start;
  }

  &__content {
    display: grid;
    place-content: start;
    place-items: start;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    row-gap: var(--space-2xl);
    column-gap: var(--space-ml);
  }
}
</style>
