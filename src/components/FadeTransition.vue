<template>
  <Transition name="fade">
    <slot />
  </Transition>
</template>

<style>
.fade-enter-active,
.fade-leave-active {
  transform-origin: unset;
  transition: opacity 0.5s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
</style>
