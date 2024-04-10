<template>
  <div class="dropback-circle">
    <div class="dropback-circle__background"></div>
    <div class="dropback-circle__content">
      <TelegramIcon />
      <InstagramIcon />
      <LinkedInIcon />
    </div>
  </div>
</template>

<script setup lang="ts">
import TelegramIcon from '../../assets/icons/TelegramIcon.vue'
import InstagramIcon from '../../assets/icons/InstagramIcon.vue'
import LinkedInIcon from '../../assets/icons/LinkedInIcon.vue'
</script>

<style scoped lang="scss">
.dropback-circle {
  position: fixed;
  top: 320px;
  right: 85%;
  width: 324px;
  height: 324px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;

  &__content {
    display: flex;
    flex-direction: column;
    gap: var(--space-sm);
    align-items: center;
    justify-content: center;
  }

  &__background {
    position: fixed;
    top: 320px;
    right: 85%;
    z-index: 0;
    display: block;
    background-color: var(--color-accent-main);
    filter: blur(240px);
    width: 424px;
    height: 424px;
    border-radius: 50%;
  }
}
</style>
