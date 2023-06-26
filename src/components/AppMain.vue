<template>
    <main>
        <AppLanding />
        <AppConsultants />
        <AboutUs />
    </main>
</template>

<script>
import AppLanding from './main/AppLanding.vue';
import AppConsultants from './main/AppConsultants.vue';
import AboutUs from './main/AboutUs.vue';

export default {
    name: 'AppMain',
    components:{
        AppLanding,
        AppConsultants,
        AboutUs
    }
}
</script>

<style lang="">
    
</style>