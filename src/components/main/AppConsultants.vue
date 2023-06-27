<template>
    <section class="consultants">
        <div class="background">

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

        .background{
            height: 100%;
            background-color: $white-bg;
        }
    }
</style>