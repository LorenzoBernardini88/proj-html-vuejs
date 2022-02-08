<template>
    <header>
        <div class="top_head">
            <div class="ms_container">
                <span class="weekly_working_hours"><i class="fas fa-clock"></i> Open Hours: Mon-Sat-9:00-18:00 </span>
                <ul class="contacts">
                    <li><i class="fas fa-phone-alt"></i> +1(305) 1234-5678</li>
                    <li><i class="fas fa-envelope"></i> hello@example.com</li>
                    <li><i class="fab fa-facebook-f"></i></li>
                    <li><i class="fab fa-twitter"></i></li>
                    <li><i class="fab fa-linkedin-in"></i></li>
                </ul>
            </div>

        </div>

    </header>
</template>

<script>
export default {
    name: 'Header'

}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.top_head{
    background:$bg_top_head;
    padding: 20px;
    .ms_container{
        color:#FFFFFF ;
        display:flex;
        align-items: center;
        justify-content: space-between;
        font-size: 12px;
        font-weight: 100;
        ul{
            display: flex;
            align-items: center;
            gap: 20px;
            list-style-type: none;
            margin: 0;
        }
    }
}
</style>