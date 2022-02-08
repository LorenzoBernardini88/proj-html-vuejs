<template>
    <div class="ms_sec_cont">
        <div class="text_cont">

        <h6>introduction video</h6>
        <h1>Advisory <span class="title_evidence">Performance</span></h1>
        <p>Financial executives need to review thier strategies, operating models and capabilities so that their areas can genrate sound information for better decision making</p>
        </div>
        <div class="img_video_cont">
            <img src="../../assets/video-1.jpg" alt="">
        </div>
    </div>
</template>

<script>
export default {
    name: "VideoIntro"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.ms_sec_cont{
    
    padding: 50px 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap:20px;

    .text_cont{
        width: 90%;
        margin: 0 auto;
        text-align: center;
        display: flex;
        flex-direction: column;
        gap: 20px;

        p{
            font-size:$size_p;
            color:#808080
            
        }
    }
        
    .img_video_cont{
        width: 100%;
        height: 300px;
        
        img{
            width: 100%;
            height: 100%;
        }
    }
}
</style>