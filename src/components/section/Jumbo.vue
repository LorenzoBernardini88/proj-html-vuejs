<template>
    <div class="jumbo">
        <!-- <img class="img_slide" v-for="(image,indice) in imgJumbo" :key="indice" :src="image" alt=""> -->
        <div class="jumbo_cont">
            <h1>Financial Risk</h1>
            <p>The right outcomes depend on continuous rigor in governance, models, and processes across the finance function</p>
            <div class="buttons_jumbo">
                <a class="button_green" href="#">GET IN TOUCH</a>
                <a id="btn_read" class="empty_button" href="#" :class="{color_hover : hover}" @mouseover="hover=true" @mouseleave="hover=false" >READ MORE</a>
            </div>
        </div>
        <div class="ms_container">
            <img src="../../assets/nexgen-logo.svg" alt="">
            <ul>
                <li href="#" v-for="(elemento,index) in dataNav" :key="index">{{elemento.text}}</li>
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
            dataNav : data,
            hover : false,
            element: "",
            corrente : 0,
            imgJumbo:[
                require("../../assets/bg_img/bg-1.jpg"),
                require("../../assets/bg_img/bg-3.jpg")
            ]
        }
    },
    
}
</script>


<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.jumbo{
    min-height: 600px;
    background: rgba(0, 0, 0,0.5);
    position: relative;
    
    &::before{
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background-image: url("../../assets/bg_img/bg-2.jpg");
        background-size: cover;
        background-repeat: no-repeat;
        z-index:-1;
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
            font-size: 16px;
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
            margin: 0;
        }

        p{
            font-size: $size_p;
            font-weight: 100;
            margin: 30px 0 ;
        }
        a.empty_button{
            margin-left:20px;
        }
    }
}
</style>




