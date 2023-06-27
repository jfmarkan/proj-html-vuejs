<template>
    <footer>
        <div class="container">
            <div class="footer-top">
                <div class="logo">
                    <img src="../assets/img/logotype-2-139x23.png" alt="">
                </div>
                <div>
                    <ul>
                        <li v-for="link in menuLinks">
                            {{link.text}}
                        </li>
                    </ul>
                </div>
                <div class="social">
                    <div class="icon">
                        <i class="fa-brands fa-instagram"></i>
                    </div>
                    <div class="icon">
                        <i class="fa-brands fa-linkedin-in"></i>
                    </div>
                    <div class="icon">
                        <i class="fa-brands fa-facebook-f"></i>
                    </div>
                    <div class="icon">
                        <i class="fa-brands fa-twitter"></i>
                    </div>
                </div>
            </div>
            <hr>
            <div class="footer-bottom">
                <div>
                    <a href="">Terms of use</a><br>
                    <a href="">Privacy Environmental Policy</a>
                </div>
                <div>
                    <span>Copyright &copy; 2023 Plox Consulting. All Rights Reserved.</span>
                </div>
            </div>
        </div>
        
    </footer>
</template>

<script>
export default {
    name: 'AppFooter',
    props:{
        menuLinks:Array,
    }
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

    footer{
        background-color: $blue-bg;
        color:#FFFFFF;

        .footer-top{
            @include d-flex();
            padding-bottom: 80px;


            .social{
                @include d-flex(row, center, center, nowrap);
                .icon{
                    @include d-flex(row, center, center, nowrap);
                    width: 34px;
                    height: 34px;
                    &:hover{
                        cursor: pointer;
                        color: $red-bg;
                        transition: all 0.1s ease-in-out;
                    }
                }
            }
        }

        div ul{
        @include d-flex(row, space-between, center, nowrap);

            li{
                padding: 1.25rem;
                font-size: .75rem;
                line-height: 23px;
                color: #cfcfcf;
                position: relative;
                &:hover{
                    cursor: pointer;
                    color: $red-bg;
                    transition: all 0.1s ease-in-out;
                }
            }
        }

        .footer-bottom{
            @include d-flex(row, space-between, end, nowrap);
            padding-top: 35px;
            padding-bottom: 39px;

            a{
                font-weight: 400;
                font-size: 14px;
                line-height: 22px;
                text-decoration: none;
                color: #FFFFFF;
            }
        }
    }
</style>