<template>
<div class="sec_newsLetter">
    <div class="ms_sec_cont ">
        <div class="newsLetter_text">
            <h6>newsletter</h6>
            <h1><span class="title_evidence2">Know</span> First</h1>
            <p>follow closely and received content about our company and news of the current market</p>
        </div>
        <div class="input_cont">
            <input type="text" name="" id="" placeholder="Name">
            <input type="text" name="" id="" placeholder="Email">
            <a href="#" class="button_green">subscribe</a>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name:"SecLetterMain"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.sec_newsLetter{
    background:#111117;
    padding: 50px 0;
    display: flex;
    align-items: center;
    justify-content: center;
    .ms_sec_cont{
        height: 180px;
        display: flex;
        justify-content: space-between;
        .newsLetter_text{
            width: 50%;
            display: flex;
            flex-direction: column;
            justify-content: space-between;

            h1,p{
                color:#fff;
            }
            p{
                font-size: $size_p;
                font-weight: 100;
                width: 95%;
                margin: 0;
            }
        }
        .input_cont{
            width: 40%;
            display: flex;
            flex-direction: column;
            justify-content: space-around;
            a.button_green{
                width: 140px;
            }
            input{
                background:#1D1D23 ;
                color: $color_p;
                font-size:$size_p;
                font-weight: 100;
                border: none;
                padding: 10px;
                border-radius: 3px;
                width: 100%;
            }
        }
    }

}
</style>