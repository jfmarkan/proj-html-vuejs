<template>
    <header>
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

    header{
        @include d-flex(row, space-between, center, nowrap);
        width: 100%;
        height: 78px;
    }
    .logo img{
        width: 112px;
    }
</style>