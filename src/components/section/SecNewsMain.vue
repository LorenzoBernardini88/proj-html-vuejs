<template>
<div class="sec_news">
    <div class="ms_container">
        <div class="text_news">
            <h6>our editorial content</h6>
            <h1>Latest <span class="title_evidence">News</span></h1>
            <p>Every week pubblish content about what in best in the business world. </p>
            <a href="#" class="button_green">see all</a>
        </div>
        <div class="news_profile">
            <div v-for="(elemento,indice) in dataNews" :key="indice" class="photo_profile">
                <div class="overlay"></div>
                <img :src="elemento.img" alt="">
                <p>{{elemento.text}}</p>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: "SecNewsMain",
    data(){
        return{
            dataNews:[
                {
                    img: require("../../assets/news_img/news-1.jpg"),
                    text:"Lorem ipsum dolor sit amet, consectetur.",
                },
                {
                    img: require("../../assets/news_img/news-2.jpg"),
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
                },
                {
                    img: require("../../assets/news_img/news-3.jpg"),
                    text: "Lorem ipsum dolor sit amet, consectetur.",
                }
                
            
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.sec_news{
    background:#E7EEE9 ;
    min-height:400px ;
    padding: 50px 0px;
    
    .text_news{
        position: relative;
        h1{
            margin: 30px 0;
        }
        p{
            font-size: $size_p;
            color: #808080;
        }
        a{
            position: absolute;
            bottom: 0;
            right: 0;

        }
    }
    .news_profile{
        padding-top:20px;
        display: flex;
        justify-content: space-between;

        .photo_profile{
            width: 30%;
            text-align: center;
            position: relative;
            p{
                width: 80%;
                font-size: 18px;
                color: #fff;
                font-weight: bold;
                position: absolute;
                bottom: 10px;
                right: 30px;
            }
            img{
                width: 100%;
                border-radius: 10px;
                object-fit: cover;
            }
            .overlay{
                position: absolute;
                width: 100%;
                height: 100%;
                bottom: 0;
                left: 0;
                right: 0;
                top: 0;
                border-radius: 10px;
                background: rgba(0,0,0,0.4);
            }
        }
        
    }
}
</style>
