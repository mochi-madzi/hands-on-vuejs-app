<template>
  <img class="vuetify-logo" alt="Vuetify Logo" src="/vuetify-logo.svg" />
</template>

<style>
.vuetify-logo {
  height: 280px;
  width: 280px;
  transform: rotateY(560deg);
  animation: turn 3.5s ease-out forwards 1s;
}

@keyframes turn {
  100% {
    transform: rotateY(0deg);
  }
}
</style>
