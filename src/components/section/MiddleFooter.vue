<template>
    <div class="middle_footer">
        <div class="ms_container">
            <div class="ms_card card1">
                <img src="../../assets/nexgen-logo.svg" alt="">
                <p>A functional HTML Template for Comporate & Business</p>
                <p v-for="(elemento,indice) in dataCard1" :key="indice"><i :class="elemento.icon"></i> {{elemento.info}}</p>
                <a href="#" class="empty_button" :class="{color_hover :hover}" @mouseover="hover = true" @mouseleave="hover = false">get in touch</a>
            </div>
            <div class="ms_card card2">
                <h5>About</h5>
                <ul>
                    <li v-for="(card2,indice) in dataCard2" :key="indice"><i class="fa-solid fa-angle-right"></i> {{card2}}</li>
                </ul>
            </div>
            <div class="ms_card card3">
                <h5>Services</h5>
                <ul>
                    <li v-for="(card3,indice) in dataCard3" :key="indice"><i class="fa-solid fa-angle-right"></i> {{card3}}</li>
                </ul>
            </div>
            <div class="ms_card card4">
                <h5>Support</h5>
                <ul>
                    <li v-for="(card4,indice) in dataCard4" :key="indice"><i class="fa-solid fa-angle-right"></i> {{card4}}</li>
                </ul>
            </div>
            
        </div>
    </div>
</template>

<script>
export default {
    name: "MiddleFooter",
    data(){
        return {
            dataCard1 : [
                {
                    icon: "fas fa-phone-alt",
                    info: "+1(305) 1234-5678"
                },
                {
                    icon: "fas fa-envelope",
                    info: "hello@example.com"
                },
                {
                    icon: "fa-solid fa-location-dot",
                    info: "Main Avenue, 987"
                }
            ],
            dataCard2: [
                "The Company",
                "Institutional",
                "Social & Events",
                "Innovation",
                "Environment",
                "Technology"
            ],
            dataCard3: [
                "Audit & Assurance",
                "Financial Advisory",
                "Analytics M&A",
                "Middle Marketing",
                "Legal Consulting",
                "Regulatory Risk"
            ],
            dataCard4: [
                "Responsibility",
                "Terms of Use",
                "About Cookies",
                "Privacy Policy",
                "Accessibility",
                "Information"
            ],
            hover : false
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.middle_footer{
    min-height: 500px;
    padding: 50px 0;
    background-image:url("../../assets/bg_img/bg-7.jpg");
    background-size: cover;
    background-position: center;
    display: flex;
    justify-content:center;
    align-items:center;

    .ms_container{
        display: flex;
        justify-content: space-between;
        .ms_card{
            width: 22%;
            color:#BCBDBD;
            h5{
                color:#fff;
                font-weight: bold;
                margin-bottom: 20px;

            }
            ul{
                list-style-type: none;
                padding: 0;
                
                li{
                    font-weight: 300;
                    font-size: 15px;
                    line-height: 30px;

                    svg{
                        display:inline-block;
                        margin-right: 10px;
                    }
                }
            }
        }
        .card1{
            font-size: 15px;
            img{
                width: 150px;
                margin-bottom: 25px;
            }
            a.empty_button{
                display: inline-block;
                margin-top: 15px;
            }
        }
        .card2,
        .card3,
        .card4{
            background: rgba(103, 102, 105,0.1);
            padding:30px;
            border-radius: 10px;
        }
    }
}
</style>
