<script>
import AppHeader from './components/AppHeader.vue';
import '@fortawesome/fontawesome-free/css/all.css';
import AppjumbotronVue from './components/Appjumbotron.vue';
export default{
  data(){
    return{
      
    }
  },
  components:{
    AppHeader,
    AppjumbotronVue
  }
}
</script>

<template>
  <div>
    <AppHeader></AppHeader>
    <AppjumbotronVue></AppjumbotronVue>
  </div>
</template>

<style lang="scss" scoped>

</style>
