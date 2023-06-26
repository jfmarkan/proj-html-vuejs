<template>
    <AppHeader />
    <AppMain />
    <AppFooter />
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
                    "text": "HOME",
                    "link": "#",
                },
                {
                    "text": "ABOUT",
                    "link": "#",
                },
                {
                    "text": "PROJECTS",
                    "link": "#",
                },
                {
                    "text": "SERVICES",
                    "link": "#",
                },
                {
                    "text": "BLOG",
                    "link": "#",
                },
                {
                    "text": "CONTACT",
                    "link": "#",
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