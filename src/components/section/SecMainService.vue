<template>
<div class="sec_service">
    <div class="ms_container">
        <div class="text_service">
            <h6>our business areas</h6>
            <h1>Excellence in<span class="title_evidence2"> Service</span></h1>
            <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowned professionals. These are some options that you can hire.</p>
            <a href="#" class="empty_button">see all</a>
        </div>
        <div class="card_service_cont">
            <CardService
            v-for="elemento in dataService" 
            :key="elemento.id"
            :servizio="elemento"/>
        </div>
    </div>
</div>
</template>



<script>
import CardService from "../commons/CardService.vue"
export default {
    name:"SecMainService",
    components:{
        CardService
    },
    data(){
        return{
            dataService: [
                {
                    icon:"fa-solid fa-network-wired",
                    arrow:"fa-solid fa-arrow-right",
                    title:"Audit & Assurance",
                    text:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. ",
                    id: "0"
                },
                {
                    icon:"fa-solid fa-briefcase",
                    arrow:"fa-solid fa-arrow-right",
                    title:"Financial Adivisory",
                    text:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. ",
                    id: "1"
                },
                {
                    icon:"fa-solid fa-chart-simple",
                    arrow:"fa-solid fa-arrow-right",
                    title:"Analytics and M&A",
                    text:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. ",
                    id: "2"
                },
                {
                    icon: "fa-solid fa-plane-up",
                    arrow:"fa-solid fa-arrow-right",
                    title:"Middle Marketing",
                    text:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. ",
                    id: "3"
                },
                {
                    icon:"fa-solid fa-globe-stand",
                    arrow:"fa-solid fa-arrow-right",
                    title:"Legal Consulting",
                    text:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. ",
                    id: "4"
                },
                {
                    icon:"fa-solid fa-inbox",
                    arrow:"fa-solid fa-arrow-right",
                    title:"Regulatory Risk",
                    text:"Lorem ipsum dolor sit amet, consectetur adipiscing elit. ",
                    id: "5"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.sec_service{
    min-height: 600px;
    background: #111117;
    padding: 70px 0;

    .text_service{
        position: relative;
        
        h1{
            color: #fff;
            margin: 20px 0;
        }
        p{
            width: 90%;
            color: #BCBDBD;
            font-weight: 100;
            font-size: $size_p;
        }
        a.empty_button{
            position: absolute;
            bottom:0;
            right:0;
        }
    }
    .card_service_cont{
        padding-top:30px;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }


}






</style>