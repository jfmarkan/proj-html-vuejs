<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/logotype.png" alt="">
            </div>
            <div class="navbar">
                <nav>
                    <ul>
                        <li v-for="link in menuLinks" :class="link.active ? 'active' : ''">
                            <div :class="link.active ? 'highlighted' : ''"></div>
                            {{link.text}}
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
        @include d-flex();
        width: 100%;
        height: 78px;

        .container{
            @include d-flex();
        }
    }
    .logo img{
        width: 112px;
    }

    nav ul{
        @include d-flex(row, space-between, stretch, nowrap);

        li{
            padding: 1.25rem;
            font-size: 15px;
            line-height: 23px;
            color: #cfcfcf;
            position: relative;
        }
            .active{
                font-weight: 700;
                color: #FFFFFF;
            }

            div.highlighted{
                width: calc(100% - 2.5rem);
                height: 3px;
                background-color: #FFFFFF;
                position: absolute;
                top: 0;
            }
        
    }
</style>