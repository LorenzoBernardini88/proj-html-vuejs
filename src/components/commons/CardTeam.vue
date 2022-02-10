<template>
<div class="cardTeam_cont">
    <div class="profile_photo">
        <img :src="team.img" alt="">
    </div>
    <div class="text_card">
        <div>{{team.name}}</div>
        <p>{{team.role}}</p>
        <ul>
            <li v-for="(elemento,indice) in iconArray" :key="indice"><i :class="elemento"></i></li>
        </ul>
    </div>
</div>
</template>

<script>
export default {
    name : "CardTeam",
    props:{
        team: Object
    },
    data(){
        return{
            iconArray: [
            "fa-brands fa-facebook-f social",
            "fa-brands fa-twitter social",
            "fa-brands fa-linkedin-in social"
            ],
            
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.cardTeam_cont{
    width: 45%;
    height: 140px;
    display: flex;
    gap: 20px;
    
    .profile_photo{
        width: 50%;
        border-radius: 5px;
        img{
            border-radius: 5px;
            width: 100%;
            height: 100%;
            
        }
    }
    .text_card{
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        width: 50%;
        height: 100%;

        div{
            font-weight:600;
        }
        p{
            color: $color_p;
            margin-top: 10px;
            font-size: 12px;
            text-transform: uppercase;
        }
        ul{
            list-style-type: none;
            display: flex;
            gap: 20px;
            text-align: left;
            padding: 0;

            
        }
    }
}
    
</style>