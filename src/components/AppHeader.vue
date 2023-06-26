<template>
    <header>
        <div>
            <div class="container">
                <div class="logo">
                    <img src="../assets/img/logotype.png" alt="">
                </div>
                <div class="navbar">
                    <nav>
                        <ul>
                            <li v-for="menulink in menuLinks">
                                {{ menulink.text }}
                            </li>
                        </ul>
                    </nav>
                </div>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'AppHeader',
    props:{
        menuLinks : Array,
    }
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

    .logo img{
        width: 112px;
    }
</style>