<template>
    <section class="consultants">
        <div class="align-right">
            <div class="spacer"></div>
            <div class="background">
                <div class="section-title">
                    <p class="title-text">OUR CONSULTANTS CAN HELP YOU</p>
                    <div class="green-line"></div>
                </div>
                <div class="content">
                    <div class="row">
                        <div class="single-consultant">
                            <div class="icon">
                                <img src="https://demo.phlox.pro/consulting-2/wp-content/uploads/sites/113//2019/06/line-graph.svg" alt="">
                            </div>
                            <div>
                                <p class="title">STATISTICAL CONSULTING</p>
                                <p class="description">When, while lovely valley teems with vapour arround meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
                            </div>
                        </div>
                        <div class="single-consultant">
                            <div class="icon">
                                <img src="https://demo.phlox.pro/consulting-2/wp-content/uploads/sites/113/2019/06/shout.svg" alt="">
                            </div>
                            <div>
                                <p class="title">DIGITAL CONSULTING</p>
                                <p class="description">When, while lovely valley teems with vapour arround meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
                            </div>
                        </div>
                    </div>
                    <div class="row">
                        <div class="single-consultant">
                            <div class="icon">
                                <img src="https://demo.phlox.pro/consulting-2/wp-content/uploads/sites/113//2019/06/Path-13.svg" alt="">
                            </div>
                            <div>
                                <p class="title">BANKING CONSULTING</p>
                                <p class="description">When, while lovely valley teems with vapour arround meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
                            </div>
                        </div>
                        <div class="single-consultant">
                            <div class="icon">
                                <img src="https://demo.phlox.pro/consulting-2/wp-content/uploads/sites/113/2019/06/target.svg" alt="">
                            </div>
                            <div>
                                <p class="title">ENTERPRISE CONSULTING</p>
                                <p class="description">When, while lovely valley teems with vapour arround meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppConsultantsg'
}
</script>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

    .align-right{
        @include d-flex();
    }
    div.spacer{
        width: 8%;
    }
    div.background{
        width: 92%;
        height: 94vh;
        background-color: #FFF;    
        .section-title{
            @include d-flex(row, end, center, nowrap);
            margin: 7rem 0;
            font-family: 'Bai Jamjuree', sans-serif;
            font-size: 30px;
            .title-text{
                margin-right: 2rem;
            }
            .green-line{
                width: 58%
            }
        }
        .content{
            width: 100%;
            height: 100%;
            
            .row{
                @include d-flex(row, space-around, start, wrap);
                margin: 10rem 0;
            
            .single-consultant{
                @include d-flex(row, center, start, nowrap);
                width: 30%;
                margin-left: 8rem;
                .icon{
                    @include d-flex(row, center, center, nowrap);
                    background-color: $red-bg;
                    border-radius: 50%;
                    padding: 1rem;
                    width: 65px;
                    height: 65px;
                    margin-right: 3rem;

                }
                .title{
                    font-family: 'Bai Jamjuree', sans-serif;
                    margin: .5rem 0 1rem;
                }
            }
        }
    }
}

    
</style>