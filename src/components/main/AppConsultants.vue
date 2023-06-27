<template>
    <section class="consultants">
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
    name: 'AppConsultantsg'
}
</script>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

    section{
        height: 94vh;
    }
    .align-right{
        @include d-flex();
    }
    div.spacer{
        width: 9%;
    }
    div.background{
        width: 91%;
        height: 94vh;
        background-color: #FFF;
    }
    .testimonials{
        @include d-flex();
        width: 90%;
    }
    .content{
        @include d-flex(row, center, center, nowrap);
        position: absolute;
        width: 95%;
        height: 100%;
    }
</style>