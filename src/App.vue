<script>
import TheHeader from './components/TheHeader.vue';
import TheMain from './components/TheMain.vue';
import BlueBar from './components/BlueBar.vue';
import TheFooter from './components/TheFooter.vue';
import Cta from './components/Cta.vue';

export default {
  components: {
    TheHeader,
    TheMain,
    BlueBar,
    TheFooter,
    Cta
  },
}
</script>

<template>
  <TheHeader />
  <TheMain />
  <BlueBar />
  <TheFooter />
  <Cta />
</template>

<style lang="scss">

</style>