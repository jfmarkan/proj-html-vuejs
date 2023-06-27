<template>
    <section class="talk-work">
        <div class="img-bg">
            <div class="content">
                <h3>LET'S TALK ABOUT WORK</h3>
                <p>A wonderful serenity has taken possesion Far far away, behind the word mountains.</p>
                <button>GET STARTED</button>
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
        .content{
            @include d-flex(column, center, center, nowrap);

            p{
                text-align: center;
                line-height: 1.5rem;
                width: 23%;
                margin: 1rem 0 2rem;
            }

            button{
                padding: 1rem 2rem;
                font-size: .75rem;
                background-color: $blue-bg;
                color: $white-text;
            }
        }
        .img-bg{
            background-image: url('../../assets/img/business-people-working-together-on-project-and-B3MZ4TX.jpg');
            background-size: cover;
            background-repeat: no-repeat;
            padding: 140px 0 80px;
        }
    }
</style>