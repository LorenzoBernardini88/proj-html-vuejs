<template>
    <div class="ms_container">
        <div class="team_cont">
            <div class="text_team">
                <h6>we like what we do </h6>
                <h1><span class="title_evidence">Team</span> of Expert</h1>
                <p>Ethics and integrity are the bases on wich our profesdsionals build their careers.They are fundamentals that become daily attitudes</p>
                <div class="team_profile">
                    <card-team
                    v-for="(elemento,indice) in dataTeam"
                    :key="indice"
                    :team="elemento"/>
                </div>
            </div>
        </div>
        <div class="pres_cit">
            <div class="speech">President Speech</div>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.Praesent et enim sit</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent et enim sit amet,Lorem ipsum dolor sit amet</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.Praesent et enim sit</p>
            <p class="president">T.Johnson <i class="fa-solid fa-quote-right"></i></p>
        </div>
    </div>
</template>
            
            

<script>
import CardTeam from '../commons/CardTeam.vue'
export default {
    name: "SecTeamMain",
    components: { 
        CardTeam 
    },
    data(){
        return{
            dataTeam : [
                {
                    name:"David Cooper",
                    role: "cto & co-founder",
                    img:  require("../../assets/team_img/team-1.jpg"),
                },
                {
                    name: "Oliver Stone",
                    role: "chief procurement",
                    img:  require("../../assets/team_img/team-3.jpg"),
                },
                {
                    name: "Emma Lopez",
                    role: "chief marketing",
                    img:  require("../../assets/team_img/team-2.jpg"),
                },
                {
                    name: "T.Johnson",
                    role: "ceo & president",
                    img:  require("../../assets/team_img/team-4.jpg"),
                },
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.ms_container{
    padding: 50px 0;
    display: flex;
    justify-content: space-between;
    position: relative;
    .team_cont{
        width: 65%;
        .text_team{
            h1{
                text-align: left;
                margin:20px 0;
            }
            p{
                color:$color_p;
                font-size:$size_p;
            }
        }
        .team_profile{
            display: flex;
            flex-wrap:wrap;
            justify-content: space-between;
            gap: 10px;
        }
    }
    .pres_cit{
        width: 25%;
        background: #098081;
        color: #fff;
        padding: 20px;
        position: absolute;
        right: 0;
        bottom: 50px;

        .speech{
            font-weight: bold;
            font-size: 17px;
            margin-bottom: 15px;
        }
        p{
            font-size: 15px;
            font-weight: 200;
        }
        p.president{
            font-weight: bold;
        }
        .fa-quote-right{
            color:#676669;
            font-size: 25px;
            position: relative;
            left: 110px;
        }
    }
}
</style>

    

