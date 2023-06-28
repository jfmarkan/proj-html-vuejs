<template>
    <section class="Projects">
        <div class="container">
            <div class="intro">
                <div class="green-line"></div>
                <h5>PROJECT</h5>
            </div>
            <div class="project-selector">
            <h4>OUR EXPERT TRUSTED CONSULTANTS <br> HELP CLIENTS</h4>
            <div class="arrows">
                <div class="arrow">
                <i class="fa-solid fa-arrow-left"></i>
            </div>
            <div class="arrow">
                <i class="fa-solid fa-arrow-right"></i>
            </div>
            </div>
            
            </div>
            
            <div class="content">
                <div class="action">
                    <div class="single-project">
                        <img src="../../assets/img/DRY-1-790x592.jpg" alt="">
                    </div>
                    <div class="single-project">
                        <img src="../../assets/img/221bf0b7-8134-43bb-936a-5acbe42db64a-790x592.jpg" alt="">
                    </div>
                    <div class="single-project">
                        <img src="../../assets/img/z1el4c4p-790x592.jpg" alt="">
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppProjects'
}
</script>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

    section{
        background-color: $blue-bg;
        color:#FFFFFF;
        margin-top: 220px;

        .intro{
            @include d-flex(row, start, baseline, nowrap);
            margin-bottom: 1rem
        }
        .project-selector{
            @include d-flex();
        }
        .arrows{
            @include d-flex();
            .arrow{
                @include d-flex(row, center, center, nowrap);
                width: 50px;
                height: 50px;
                background-color: rgba(33,150,243,.2);
                margin: .25rem;
                &:hover{
                    background-color: $green-bg;
                }
            }
        }
        .content{
            @include d-flex(column, center, center, nowrap);
            margin-top: 2rem;
        }
        .img-bg{
            background-image: url('../../assets/img/business-people-working-together-on-project-and-B3MZ4TX.jpg');
            background-size: cover;
            background-repeat: no-repeat;
            padding: 140px 0 80px;
        }

        .action {
            @include d-flex();
            .single-project{
                position: relative;
                width: calc((100% / 3) - 1rem);
                overflow: hidden;
                img{
                    width: 100%;
                }
                &:hover{
                    img{
                        transform: scale(1.2);
                        transition: all 1s ease-in-out;
                    }
                    &::after{
                        background-color: #f00e2e;
                        z-index: 1;
                        content: '';
                        display: block;
                        width: 100%;
                        height: 100%;
                        mix-blend-mode: darken;
                        position: absolute;
                        top: 0;
                        left: 0;
                    }
                }
            }
        }
    }
</style>