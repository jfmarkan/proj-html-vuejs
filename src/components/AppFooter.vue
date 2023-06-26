<template>
    <footer>
        <div class="container">
            <div>
                <div>
                    <img src="../assets/img/logotype-2-139x23.png" alt="">
                </div>
                <div>
                    <i class="fa-brands fa-instagram"></i>
                    <i class="fa-brands fa-linkedin-in"></i>
                    <i class="fa-brands fa-facebook-f"></i>
                    <i class="fa-brands fa-twitter"></i>
                </div>
            </div>
            <hr>
            <div>
                <ul>
                    <li>

                    </li>
                </ul>
            </div>
            <hr>
            <div>
                <div>
                    <a href="">Terms of use</a>
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
    name: 'AppFooter'
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

    footer{
        background-color: $blue-bg;
        color:#FFFFFF;
    }
</style>