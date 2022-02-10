<template>
<div class="card_serv">
    <div class="icon_cont">
        <span class="icon"><i :class="servizio.icon"></i></span>
        <span class="arrow"><i :class="servizio.arrow"></i></span>
    </div>
    <div class="text_service">
        <div class="title">{{servizio.title}}</div>
        <div class="pharag">{{servizio.text}}</div>
    </div>
</div>
</template>

<script>
export default {
    name: "CardService",
    props:{
        servizio: Object
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.card_serv{
    width: 30%;
    height: 200px;
    border-radius: 10px;
    background:#1D2528;
    padding:30px;
    margin-bottom: 40px ;

    .icon_cont{
        display: flex;
        justify-content: space-between;
        span.icon{
        font-size: 30px ;
        color:#098081;
        }
        span.arrow{
            color:#048383;
            }
    }
    .text_service{
        width: 90%;
        .title{
            color: #fff;
            font-weight: bold;
            margin: 10px 0;
        }
        .pharag{
            color: #BCBDBD;
            font-size: 13px;
            font-weight: 300;
        }

    }

}

</style>