<template>
    <main>
        <AppLanding />
        <AppConsultants />
        <AppAboutUs />
        <AppBusinessCase />

        <AppTalk />
    </main>
</template>

<script>
import AppLanding from './main/AppLanding.vue';
import AppConsultants from './main/AppConsultants.vue';
import AppAboutUs from './main/AppAboutUs.vue';
import AppBusinessCase from './main/AppBusinessCase.vue';
import AppTalk from './main/AppTalk.vue';

export default {
    name: 'AppMain',
    components:{
        AppLanding,
        AppConsultants,
        AppAboutUs,
        AppBusinessCase,

        AppTalk
    }
}
</script>

<style lang="">
    
</style>