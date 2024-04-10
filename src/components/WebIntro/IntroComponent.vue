<template>
  <div class="heading">
    <div class="heading--left">
      <p>LET US BUILD <span>YOUR DREAM</span></p>
      <VerticalBar />
    </div>
    <div class="heading--right">
      <h1>
        WEB &amp; SOFTWARE<br />
        DEVELOPMENT
      </h1>
      <HorizontalBar :width="100" />
      <p>
        “Resolute devs” - is a team of professionals specializing in creating<br />
        web applications with maximum speed and quality. We offer a full<br />
        range of services for the development, maintenance, promotion of<br />
        websites and software.
      </p>
    </div>
  </div>
</template>

<script setup lang="ts">
import VerticalBar from '../../assets/icons/VerticalBar.vue'
import HorizontalBar from '../../assets/icons/HorizontalBar.vue'
</script>

<style scoped lang="scss">
.heading {
  color: white;
  display: flex;
  flex-direction: row;
  gap: var(--space-m);
  margin-top: var(--space-3xl);
  align-self: flex-end;

  &--left {
    font-family: var(--font-roboto-bold);
    font-size: var(--font-size-p2-pc-tablet);
    color: var(--color-grey-main);
    display: flex;
    flex-direction: row;
    gap: var(--space-m);
    align-items: start;
    justify-content: start;

    span {
      color: var(--color-accent-main);
    }
  }

  &--right {
    padding-left: var(--space-s);
    display: flex;
    flex-direction: column;
    gap: var(--space-m);

    h1 {
      font-family: var(--font-roboto-bold);
      font-size: var(--font-size-h1-pc);
      color: var(--color-white-main);
      line-height: 100%;
      margin-top: -10px;
    }

    p {
      font-family: var(--font-roboto-regular);
      font-size: var(--font-size-p1-pc-tablet-mobile);
      line-height: 145%;
      color: var(--color-grey-main);
    }
  }
}
</style>
