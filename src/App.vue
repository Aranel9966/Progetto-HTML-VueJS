<script>
import AppHeader from './components/AppHeader.vue';
import '@fortawesome/fontawesome-free/css/all.css';
import AppjumbotronVue from './components/Appjumbotron.vue';
import AppCard from './components/AppCard.vue';
export default{
  data(){
    return{
      
    }
  },
  components:{
    AppHeader,
    AppjumbotronVue,
    AppCard
  }
}
</script>

<template>
  <div>
    <AppHeader></AppHeader>
    <AppjumbotronVue></AppjumbotronVue>
    <AppCard></AppCard>
  </div>
</template>

<style lang="scss" scoped>

</style>
