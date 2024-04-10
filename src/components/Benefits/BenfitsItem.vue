<template>
  <div class="benefits-item">
    <h3>
      <slot name="header"></slot>
    </h3>
    <p>
      <slot name="content"> </slot>
    </p>
  </div>
</template>

<style scoped lang="scss">
.benefits-item {
  display: flex;
  flex-direction: column;
  align-items: start;
  justify-content: start;
  gap: var(--space-s);
  border: 1px solid var(--color-grey-main);
  border-radius: 14px;
  padding: var(--space-s);
  transition: all 0.3s ease;
  height: 100%;

  h3 {
    font-family: var(--font-roboto-bold);
    font-size: var(--font-size-h3-pc-tablet-mobile);
    line-height: 145%;
    color: var(--color-white-main);
  }

  p {
    font-family: var(--font-roboto-regular);
    font-size: var(--font-size-p1-pc-tablet-mobile);
    line-height: 145%;
    color: var(--color-grey-main);
  }

  &:hover {
    box-shadow: 0px 0px 20px 5px var(--color-accent-main);
  }
}
</style>
