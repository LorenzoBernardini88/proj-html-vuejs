<template>
<div class="sec_message">
    <div class="ms_container">
        <div class="write_mess_cont">
            <div class="tex_cont">
                <h6>send a message</h6>
                <h1>Get in <span class="title_evidence">Touch</span></h1>
                <p>We will responde to your message as soon as possible</p>
            </div>
            <div class="input_cont">
                <input class="name" type="text" placeholder="Name">
                <input class="mail" type="text" placeholder="Mail">
                <input class="phone" type="text" placeholder="Phone">
                <select class="info" >
                    <option value="" disabled selected hidden>More Info</option>
                </select>
                <textarea class="write_mess" placeholder="Message"></textarea>
                <a href="#" class="button_green">send</a>
            </div>
        </div>
        <div class="example_cont">
            <h5 class="example">Example Inc.</h5>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
            <ul>
                <li v-for="(elemento,indice) in dataMessage" :key="indice"><i :class="elemento.icon"></i>{{elemento.info}}</li>
            </ul>
            <a href="#" class="empty_button">view map</a>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name:"SecMessTopFooter",
    data(){
        return{
            dataMessage: [
                {
                    icon: "fas fa-phone-alt social",
                    info: "+1(305) 1234-5678"
                },
                {
                    icon: "fas fa-envelope social",
                    info: "hello@example.com"
                },
                {
                    icon: "fa-solid fa-location-dot social",
                    info: "Main Avenue, 987"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/vars.scss";
.ms_container{
    padding: 50px 0;
    display:flex;
    justify-content: space-around;
    .write_mess_cont{
        width: 50%;
        h1{
            margin: 20px 0;
        }
        p{
            color: #808080;
            font-size: $size_p;
        }
        .input_cont{
            width: 100%;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 10px 10px;
            
            input,
            textarea,
            select{
                background: #ECECEC;
                border: none;
                padding: 10px;
                border-radius: 3px;
                font-size: $size_p;
                font-weight: 200;
            }
            .name,
            .mail,
            .phone,
            .info{
                width: 245px;
            }
            .info > option{
                color:#808080;
            }
            .write_mess{
                width: 100%;
            }
        }
    }
    .example_cont{
        width: 35%;
        
        h5{
            font-weight: 600;
        }
        p{
            color: #808080;
            font-size: $size_p;
        }
        ul{
            list-style-type: none;
            padding:0;
            

            li {
                display: flex;
                align-items: center;
                gap: 10px;
                margin-bottom: 20px;
                font-size: $size_p;
                color: #048383;
            }
        }
        a.empty_button{
            color: #048383;
        }
    }

}
</style>