<script>
import AppFooter1 from './components/AppFooter1.vue';
import AppFooter2 from './components/AppFooter2.vue';
import AppHeader from './components/AppHeader.vue';
import AppJumbotron from './components/AppJumbotron.vue';
import AppMainContent from './components/AppMainContent.vue';

export default{
  data(){
    return{

    }
  },
  components: {
    AppHeader,
    AppJumbotron,
    AppMainContent,
    AppFooter1,
    AppFooter2,
  }
}

</script>



<template>

  <AppHeader/>
  <AppJumbotron/>
  <AppMainContent/>
  <AppFooter1/>
  <AppFooter2/>
 
</template>



<style>

</style>
