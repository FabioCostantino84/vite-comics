<script>
import AppHeader from './components/AppHeader.vue';
import AppJumbotron from './components/AppJumbotron.vue';
import AppMainMenu from './components/AppMainMenu.vue';
import AppFooter1 from './components/AppFooter1.vue';
import AppFooter2 from './components/AppFooter2.vue';

export default{

  name: 'App',
  data(){
    return{

    }
  },
  components: {  // ogni import che faccio vanno inseriti nei components
    AppHeader,
    AppJumbotron,
    AppMainMenu,
    AppFooter1,
    AppFooter2,
  }
}

</script>



<template>

  <AppHeader/>
  <AppJumbotron/>
  <AppMainMenu/>
  <AppFooter1/>
  <AppFooter2/>
 
</template>



<style lang="scss" scoped>

@use './assets/scss/partials/variables.scss' as *;

</style>
