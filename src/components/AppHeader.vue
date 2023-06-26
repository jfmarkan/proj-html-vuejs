<template>
    <header>
        <div class="container-fluid">
            <div class="row d-flex justify-content-between">
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
    .logo img{
        width: 112px;
    }
</style>