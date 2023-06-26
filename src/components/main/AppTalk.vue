<template>
    <section class="talk-work">
        <div class="img-bg">
            <div class="content">
                <h3>LET'S TALK ABOUT WORK</h3>
                <p>A wonderful serenity has taken possesion Far far away, behind the word mountains.</p>
                <button></button>
            </div>    
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppTalk'
}
</script>

<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
@use '../../styles/partials/mixins' as *;

    section{
        background-color: $blue-bg;
        color:#FFFFFF;
        margin: 50px 0 60px;
        padding: 140px 0 80px;

        .img-bg{
            background-image: url('../../assets/img/business-people-working-together-on-project-and-B3MZ4TX.jpg');
        }
    }
</style>