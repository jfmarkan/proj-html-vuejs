<template>
    <section class="testimonial">
        <div class="container">
            <div class="align-right-top">
                <div class="intro">
                    <h5>TESTIMONIAL</h5>
                    <div class="green-line"></div>
                </div></div>
            <h4>WHAT'S THE CUSTOMER SAY <br> ABOUT OUR WORK</h4>
        </div>
        <div class="align-right">
            <div class="spacer"></div>
            <div class="background">
                <div class="testimonials">
                    <div class="testimony">
                        <p class="speach">When, while lovely valley teems with vapour arround meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little.</p>
                        <p class="name">Vera Duncan</p>
                        <p class="enterprise">Amazon Inc.</p>
                    </div>
                    <div class="testimony">
                        <p class="speach">When, while lovely valley teems with vapour arround meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little.</p>
                        <p class="name">Vera Duncan</p>
                        <p class="enterprise">Amazon Inc.</p>
                    </div>
                    <div class="testimony">
                        <p class="speach">When, while lovely valley teems with vapour arround meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little.</p>
                        <p class="name">Vera Duncan</p>
                        <p class="enterprise">Amazon Inc.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppTestimonials'
}
</script>

<style lang="scss" scoped>
@use '../../styles/partials/mixins' as *;
@use '../../styles/partials/variables' as *;

    section{
        height: 34vh;
        margin-top: 160px;
        margin-bottom: 260px;
    }

    h4{
        text-align: right
    }
    .align-right-top{
        @include d-flex(row, end, start, nowrap)
    }

    .intro{
        @include d-flex(row, space-between, baseline, nowrap);
        width: 55%;
        margin-bottom: 1rem
    }
    .align-right{
        @include d-flex();
    }
    div.spacer{
        width: 8%;
    }
    div.background{
        width: 92%;
        height: 100%;
        background-color: #FFF;
        position: relative;
        margin-top: 2rem;
    }
    .testimonials{
        @include d-flex();
        width: 90%;
    }
    .testimony{
        width: calc((100%/3) - 2rem);
        padding: 3rem 4rem 4rem;

        .speach{
            font-size: 14px;
            
        }
        .name{
            font-family: 'Bai Jamjuree', sans-serif;
            font-size: 25px;
            margin: 55px 0 10px;
        }

        .enterprise{
            font-size: 15px
        }
    }

    .content{
        @include d-flex(row, center, center, nowrap);
        position: absolute;
        width: 95%;
        height: 100%;
    }

</style>