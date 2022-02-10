<template>
    <div class="bottom_footer">
        <div class="ms_container">
            <p>Enjoy the low price.We are tracking any intention of piracy</p>
            <p><i class="fa-solid fa-copyright"></i> 2020 NEXGEN is Proudly Powered by <a href="#S">Coding</a></p>
        </div>
    </div>
</template>

<script>
export default {
    name: "Bottomfooter"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.bottom_footer{
    background: #111117;
    padding: 30px 0;
    .ms_container{
        display: flex;
        justify-content: space-between;
        align-content: center;
        p{
            color: #BCBDBD;
            font-size: 14px;
            margin:0;


            a{
                text-decoration: none;
                color: #098081;
            }
        }
    }
}
</style>