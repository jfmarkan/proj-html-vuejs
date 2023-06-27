<template>
    <section class="Projects">
        <div class="container">
            <div class="intro">
                <div class="green-line"></div>
                <h5>BLOG</h5>
            </div>
            <div class="project-selector">
                <h4>THE RECENT NEWS YOU MUST READ IT</h4>
                <div>
                    <button>VIEW ALL</button>
                </div>
            </div>
            <div class="content">
                <article>
                    <div class="img">
                        <img src="../../assets/img/startup-business-people-and-strategy-board-PAJ3P9K-1390x1042.jpg" alt="">
                    </div>
                    <div class="info">
                        <p class="date-author">
                            july 4, 2019 by paul
                        </p>
                        <p class="title">
                            Canadian Consulting Firm acquired by UK Giant
                        </p>
                        <p class="summary">
                            When, while lovely valley teems with vapour arround meand eridian sun strikes the upper impenetrable foliage of my trees, and but a...
                        </p>
                    </div>
                </article>
                <article>
                    <div class="img">
                        <img src="../../assets/img/business-people-working-together-on-project-and-5FHSKBL-1390.jpg" alt="">
                    </div>
                    <div class="info">
                        <p class="date-author">
                            july 4, 2019 by paul
                        </p>
                        <p class="title">
                            Canadian Consulting Firm acquired by UK Giant
                        </p>
                        <p class="summary">
                            When, while lovely valley teems with vapour arround meand eridian sun strikes the upper impenetrable foliage of my trees, and but a...
                        </p>
                    </div>
                </article>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppBlog'
}
</script>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

    section{
        background-color: $blue-bg;
        color:#FFFFFF;
        margin-top: 240px;
        margin-bottom: 250px;
        .intro{
            @include d-flex(row, start, baseline, nowrap);
            margin-bottom: 1rem
        }
        .project-selector{
            @include d-flex();

            button{
                background-color: $green-bg;
            }
        }
        
        }
        .content{
            @include d-flex(row, space-between, center, nowrap);
            margin-top: 2rem;

            article{
                width: calc((100% / 2) - 1rem);
                position: relative;

                img{
                    width: 100%;
                }

                .info{
                    position: absolute;
                    padding: 3rem 8rem 2rem 6rem;
                    background-color: #FFFFFF;
                    width: 80%;
                    transform: translateY(30%);
                    right: 0;
                    bottom: 0;

                    .date-author{
                        color: $red-bg;
                    }

                    .title{
                        font-family: 'Bai Jamjuree', sans-serif;
                        font-size: 1.8rem;
                        color:#000;
                        margin: 2rem 0;
                    }

                    .summary{
                        color: #000;
                        text-align: justify;
                    }
                }
            }
        }
        .img-bg{
            background-image: url('../../assets/img/business-people-working-together-on-project-and-B3MZ4TX.jpg');
            background-size: cover;
            background-repeat: no-repeat;
            padding: 140px 0 80px;
        }

        .action {
            @include d-flex();
            
            div{
            width: calc((100% / 3) - 1rem);
                img{
                    width: 100%;
                }
            }
        }
</style>