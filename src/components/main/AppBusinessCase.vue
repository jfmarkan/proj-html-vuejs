<template>
    <section class="businesscase">
        <div class="background">
            <button>GET STARTED</button>
            <div>
                <div class="content">
                    <div class="w-17">
                        <p>WE HELP TO DELIVER THE BUSINESS CASE</p>
                    </div>
                    <div class="w-24">
                        <p>When, while lovely valley teems with vapour arround meand eridian sun strikes the upper impenetrable foliage of my trees, and but thousand unknown</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppBusinessCase'
}
</script>

<style lang="scss" scoped>
@use '../../styles/partials/mixins' as *;
@use '../../styles/partials/variables' as *;

    section{
        height: 34vh;
    }

    div.background{
        width: 92vw;
        height: 100%;
        background-color: #35ffbf;
        position: relative;
    }

    button{
        background-color: $red-bg;
        color: $white-text;
        position: absolute;
        bottom:0;
        right: 0;
        z-index:3;
        &:hover{
            background-color: $blue-bg;
        }
    }

    .content{
        @include d-flex(row, center, center, nowrap);
        position: absolute;
        width: 95%;
        height: 100%;
    
        .w-17{
            font-family: 'Bai Jamjuree', sans-serif;
            width: 17%;
            font-size: 26px;
            line-height: 30px;
            color: $blue-bg;
            margin-right: 125px;
        }

        .w-24{
            width: 24%;
            font-size: 14px;
            margin-left: 125px;
        }
    }

</style>