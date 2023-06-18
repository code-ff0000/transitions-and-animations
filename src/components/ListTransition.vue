<template>
  <Transition name="list">
    <slot />
  </Transition>
</template>

<style>
/* we will explain what these classes do next! */
.list-enter-active,
.list-leave-active {
  transition: opacity 0.5s ease, transform .5s ease;
}

.list-enter-from {
  opacity: 0;
  transform: translateY(-10px);
}

.list-leave-to {
  opacity: 0;
  transform: translateY(10px);
}
</style>
