<template>
    <AppHeader :menuLinks="menuLinks"/>
    <AppMain />
    <AppFooter :menuLinks="menuLinks"/>
</template>

<script>
import AppHeader from './AppHeader.vue';
import AppMain from './AppMain.vue';
import AppFooter from './AppFooter.vue';

export default {
    name: 'AppContainer',
    components:{
        AppHeader,
        AppMain,
        AppFooter,
    },

    data(){
        return{
            menuLinks: [
                {
                    text: 'HOME',
                    active: true,
                },
                {
                    text: 'ABOUT',
                    active: false,
                },
                {
                    text: 'PROJECTS',
                    active: false,
                },
                {
                    text: 'SERVICES',
                    active: false,
                },
                {
                    text: 'BLOG',
                    active: false,
                },
                {
                    text: 'CONTACT',
                    active: false,
                },
            ]
        }
    }
}
</script>

<style lang="scss">
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
</style>