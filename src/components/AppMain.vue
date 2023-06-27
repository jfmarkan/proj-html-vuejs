<template>
    <main>
        <AppLanding />
        <AppConsultants />
        <AppAboutUs />
        <AppBusinessCase />
        <AppProjects />
        <AppTestimonials />
        <AppBlog />
        <AppTalk />
    </main>
</template>

<script>
import AppLanding from './main/AppLanding.vue';
import AppConsultants from './main/AppConsultants.vue';
import AppAboutUs from './main/AppAboutUs.vue';
import AppBusinessCase from './main/AppBusinessCase.vue';
import AppProjects from './main/AppProjects.vue';
import AppTestimonials from './main/AppTestimonials.vue';
import AppBlog from './main/AppBlog.vue';
import AppTalk from './main/AppTalk.vue';

export default {
    name: 'AppMain',
    components:{
        AppLanding,
        AppConsultants,
        AppAboutUs,
        AppBusinessCase,
        AppProjects,
        AppTestimonials,
        AppBlog,
        AppTalk
    }
}
</script>

<style lang="">
    
</style>