<template>
  <header>
    <div class="background"></div>
    <div class="logo">
      <LogoIcon />
    </div>
    <nav class="navbar">
      <ul>
        <li>Services</li>
        <li>Benefits</li>
        <li>How we work</li>
        <li>Portfolio</li>
        <li>Contact</li>
      </ul>
    </nav>
  </header>
</template>

<script setup lang="ts">
import LogoIcon from '@/assets/icons/LogoIcon.vue'
</script>

<style scoped lang="scss">
.background {
  position: fixed;
  z-index: 1;
  content: '';
  backdrop-filter: blur(10px);
  width: 100vw;
  height: 10%;
  top: 0;
  left: 0;
}

header {
  position: sticky;
  z-index: 200;
  top: var(--space-safe);
  width: 100%;
  padding-left: 10%;
  padding-right: 10%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;

  .logo {
    position: relative;
    z-index: 200;
  }

  .navbar {
    ul {
      display: flex;
      flex-direction: row;
      gap: var(--space-m);
      position: relative;
      z-index: 200;

      li {
        font-family: var(--font-roboto-regular);
        font-size: var(--font-size-p2-pc-tablet);
        color: var(--color-grey-main);
        transition: all 0.1s ease-in-out;

        &:hover {
          color: var(--color-white-main);
          cursor: pointer;
        }

        &:active {
          color: var(--color-accent-main);
        }
      }
    }
  }
}
</style>
