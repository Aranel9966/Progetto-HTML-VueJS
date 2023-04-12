<script>
import AppHeader from './components/AppHeader.vue';
import '@fortawesome/fontawesome-free/css/all.css';
import AppjumbotronVue from './components/Appjumbotron.vue';
import AppCard from './components/AppCard.vue';
import AppMainTop from './components/AppMainTop.vue';
export default{
  data(){
    return{
      
    }
  },
  components:{
    AppHeader,
    AppjumbotronVue,
    AppCard,
    AppMainTop
  }
}
</script>

<template>
  <div>
    <AppHeader></AppHeader>
    <AppjumbotronVue></AppjumbotronVue>
    <AppCard></AppCard>
    <AppMainTop></AppMainTop>
  </div>
</template>

<style lang="scss" scoped>

</style>
