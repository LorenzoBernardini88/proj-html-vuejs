<template>
<div class="sec_numbers">
    <div class="text_cont">
        <h6>what are we doing</h6>
        <h1><span class="title_evidence2">Result</span> in Numbers</h1>
    </div>
    <div class="ms_container">
        <div v-for="(elemento,indice) in dataNumbers" :key="indice" class="numbers_cont">
            <div class="number">{{elemento.numb}}</div>
            <div class="text_number">{{elemento.text}}</div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: "SecMainNumb",
    data(){
        return{
            dataNumbers:[
                {
                    text: "Certifications",
                    numb: "128"
                },
                {
                    text: "Employees",
                    numb: "230"
                },
                {
                    text: "Costumers",
                    numb: "517"
                },
                {
                    text: "Countries Served",
                    numb: "94"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.sec_numbers{
    min-height: 400px;
    background-image: url("../../assets/bg_img/bg-1.jpg");
    background-size: cover;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap:50px;

    h1{
        color: #ffffff;
        margin-top:20px;
        
    }
    .ms_container{
        display: flex;
        justify-content: space-around;
        
        .numbers_cont{
            width: 20%;

            .number{
                font-size: 30px;
                font-weight:500;
                color: #52BABB;
            }
            .text_number{
                color:#ffffff;
                font-weight: bold;
            }
        }
    }
}
</style>