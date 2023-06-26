<template>
  <AppContainer />
</template>

<script>
import AppContainer from './components/AppContainer.vue';


export default {
  name: 'App',
  components:{
    AppContainer
  }
}
</script>

<style lang="scss">
@use './styles/general.scss' as *;

body{
  font-family: 'Montserrat', sans-serif;
}

</style>
