<template>
    <div class="ms_container">
        <div class="team_cont">
            <div class="text_team">
                <h6>we like what we do </h6>
                <h1><span class="title_evidence">Team</span> of Expert</h1>
                <p>Ethics and integrity are the bases on wich our profesdsionals build their careers.They are fundamentals that become daily attitudes</p>
                <div class="team_profile"></div>
            </div>
        </div>
        <div class="pres_cit">
            <div class="speech">President Speech</div>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.Praesent et enim sit</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent et enim sit amet,Lorem ipsum dolor sit amet</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.Praesent et enim sit</p>
            <p class="president">T.Johnson</p>
            <i class="fa-solid fa-quote-right mark"></i>
        </div>
    </div>
</template>
            

<script>
export default {
    name: "SecTeamMain"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.ms_container{
    padding: 50px 0;
    display: flex;
    justify-content: space-between;
    
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
    }
    .pres_cit{
        width: 25%;
        background: #098081;
        color: #fff;
        padding: 20px;
        position: relative;
        .speech{
            font-weight: bold;
            font-size: $size_p;
            margin-bottom: 15px;
        }
        p{
            font-size: 12px;
            font-weight: 100;
        }
        p.president{
            font-weight: bold;
        }
        .fa-quote-right{
            color:#676669;
            font-size: 25px;
            position: absolute;
            right: 20px;
            bottom: 35px;

        }
    }

}
</style>