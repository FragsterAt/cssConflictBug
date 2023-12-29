<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" class="q-checkbox" />
    </div>
  </header>

  <main>
    <TheWelcome />
  </main>
</template>

<style scoped lang="sass">
.wrapper
  .greetings
    @apply top-0.5 left-0.5
  .green
    @apply top-px left-px right-px bottom-px
    // } // remove this bracket - and there is no bug

header
  line-height: 1.5

.logo
  display: block
  margin: 0 auto 2rem


@media (min-width: 1024px)
  header
    display: flex
    place-items: center
    padding-right: calc(var(--section-gap) / 2)
  .logo 
    margin: 0 2rem 0 0
  

  header .wrapper 
    display: flex
    place-items: flex-start
    flex-wrap: wrap
  

</style>
