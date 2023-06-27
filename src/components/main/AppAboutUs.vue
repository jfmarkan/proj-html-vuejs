<template>
    <section class="aboutus">
        <div class="background">
            <div class="w-55"></div>
            <div class="w-45"></div>
        </div>
        <div class="container">
            <div class="content">
                <div class="intro">
                    <div class="green-line"></div>
                    <h5>ABOUT US</h5>
                </div>
                <h2>WE MAKE YOUR STRATEGY WORK</h2>
                <div class="action">
                    <p>When, while lovely valley teems with vapour arround meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed when I hear <br> the buzz of the little world among the stalks, and grow familiar indescribable forms of the insects .and flies, then I feel the presence of the Almighty.</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppAboutUs'
}
</script>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

    section{
        position: relative;
    }

    h2{
        margin: 30px 0;
    }
    .background{
            @include d-flex(row, center, center, nowrap); 
            background-color: $blue-bg;
            height:88vh;
            div.w-45{
                background-image: url('../../assets/img/Group_7543.svg');
                width: 45%;
                height: 100%;

            }
            div.w-55{
                background-image: url('../../assets/img/business-people-working-together-on-project-and-5FHSKBL.jpg');
                background-size: cover;
                width: 55%;
                height: 100%;

                img{
                    width: 100%;
                }
            }
        }

        .content{
            position: absolute;
            transform: translateY(-50%);
            top: 57%;
            left: 60%;
            width: 27%;

            .intro{
                @include d-flex(row, start, baseline, nowrap);

            }
            .action{
                color: #FFFFFF;
                font-size: 16px;
                line-height: 25px;
            }
        }
</style>