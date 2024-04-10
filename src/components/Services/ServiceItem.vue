<template>
  <div class="faq-wrapper" @click="closed = !closed">
    <div class="faq-wrapper__activator">
      <div class="faq-wrapper__activator__left">
        <div class="faq-wrapper__activator__left__dot"></div>
        <p>
          <slot></slot>
        </p>
      </div>
      <div class="faq-wrapper__activator__icons">
        <slot name="icons"></slot>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped lang="scss">
.faq-wrapper {
  display: flex;
  flex-direction: column;
  width: 100%;
  align-items: start;
  justify-content: space-between;
  transition: all 0.3s ease-out;
  border: 1px solid var(--color-grey-main);
  border-radius: 14px;

  &:hover {
    border: 1px solid var(--color-grey-main);
    background-color: var(--color-grey-secondary);
  }

  &:hover &__activator {
    color: var(--color-white-main);

    &__left__dot {
      background-color: var(--color-accent-main);
      box-shadow: 0px 0px 20px 5px var(--color-accent-main);
    }

    &__icons {
      opacity: 1;
    }
  }

  &__activator {
    padding: var(--space-sm) var(--space-ml);
    display: flex;
    flex-direction: row;
    align-items: center;
    color: var(--color-grey-main);
    justify-content: space-between;
    width: 100%;
    transition: all 0.3s ease;

    &__icons {
      display: flex;
      flex-direction: row;
      align-items: center;
      justify-content: center;
      gap: var(--space-sm);
      opacity: 0;
      transition: all 0.3s ease;
    }

    &__left {
      display: flex;
      flex-direction: row;
      gap: var(--space-sm);
      align-items: center;
      justify-content: center;
      &__dot {
        width: 10px;
        height: 10px;
        border-radius: 50%;
        transition: all 0.2s ease;
        background-color: var(--color-grey-main);
      }

      p {
        font-family: var(--font-roboto-regular);
        font-size: var(--font-size-p1-pc-tablet-mobile);
        line-height: 145%;
      }
    }
  }

  &__content {
    display: flex;
    flex-direction: column;
    align-items: start;
    color: var(--color-grey-main);
    justify-content: start;
    max-width: 1000px;

    p {
      line-height: 145%;
      text-align: start;
    }
  }

  &__content {
    padding-left: var(--space-ml);
    padding-bottom: var(--space-m);
    padding-right: var(--space-ml);
    padding-top: var(--space-s);
  }
}

.v-enter-from,
.v-leave-to {
  opacity: 0;
  transform: translateY(-80px);
}

.v-enter-to,
.v-leave-from {
  opacity: 0.5;
  transform: translateY(0px);
}

$transition-duration: 0.2s;

.v-enter-active,
.v-leave-active {
  transition:
    opacity $transition-duration ease-in-out,
    transform $transition-duration ease-in-out;
}
</style>
