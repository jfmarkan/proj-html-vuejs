<template>
    <section class="landing">
        <div class="background">
            <div class="w-34">
                <img src="" alt="">
            </div>
            <div class="w-66"></div>
        </div>
        <div class="container">
            <div class="content">
                <div class="intro">
                    <div class="green-line"></div>
                    <h5>ALWAYS THE BEST WAY YOU NEED IT</h5>
                </div>
                <h1>THE BEST BUSINESS CONSULTING</h1>
                <div class="action">
                    <button type="submit">READ MORE</button>
                    <div class="play"><i class="fa-solid fa-play"></i></div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppLanding'
}
</script>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

    section{
        position: relative;
        .background{
            @include d-flex(row, center, center, nowrap); 
            background-color: $blue-bg;
            height: 100vh;
            
            div.w-34{
                background-image: url('../../assets/img/Group_7543.svg');
                width: 34%;
                height: 100%;

            }
            div.w-66{
                background-image: url('../../assets/img/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg');
                background-size: cover;
                width: 66%;
                height: 100%;

                img{
                    width: 100%;
                }
            }
        }

        .content{
            position: absolute;
            transform: translateY(-50%);
            top: 50%;
            width: 50%;

            .intro{
                @include d-flex(row, start, baseline, nowrap);
                
            }
            .action{
                button{
                    font-family: "Raleway", sans-serif;
                    background-color: $green-bg;
                    font-size: 15px;
                    line-height: 19px;
                    letter-spacing: 2px;
                    font-weight: 500;
                    padding: 2rem 4rem;
                    border: none;
                }
            }

        }
    }
</style>