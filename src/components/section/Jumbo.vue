<template>
    <div class="jumbo">
        <div class="overlay"></div>
        <div class="jumbo_cont">
            <h1>Financial Risk</h1>
            <p>The right outcomes depend on continuous rigor in governance, models, and processes across the finance function</p>
            <div class="buttons_jumbo">
                <a class="button_green" href="#">GET IN TOUCH</a>
                <a class="empty_button" href="#">READ MORE</a>
            </div>
        </div>
        <div class="ms_container">
            <img src="../../assets/nexgen-logo.svg" alt="">
            <ul>
                <li href="#" v-for="elemento in dataNav" :key="elemento">{{elemento.text}}</li>
                <li><i href="#" class="far fa-user"></i></li>
                <li><a class="button_green" href="#">GET IN TOUCH</a></li>
            </ul>
        </div>
    </div>
</template>
            

<script>
import data from "../../data/data.js"
export default {
    name: "Jumbo",
    data(){
        return{
            dataNav : data
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.jumbo{
    min-height: 600px;
    background-image: url("../../assets/bg_img/bg-2.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    .overlay{
        widows: 100%;
        height: 100%;
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background: rgba(0, 0, 0,0.3);
    }
    .ms_container{
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding:20px;

        img{
            width: 150px;
        }
        ul {
            margin:0;
            font-size: 18px;
            list-style-type: none;
            color:#FFFFFF ;
            display: flex!important;
            align-items: center;
            gap: 30px;
            
        }
    }
    .jumbo_cont{
        width: 50%;
        position: absolute;
        top:50%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: #FFFFFF;
        text-align: center;
        h1{
            font-size: 4rem ;
            font-weight: bold;
        }

        p{
            font-size: $size_p;
            font-weight: 100;
            margin: 30px 0 ;
        }

        a.button_green{
            margin-right:20px
        }
    }
}



</style>
