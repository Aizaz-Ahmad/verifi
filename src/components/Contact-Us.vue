<template>
    <div class="container">
        <div class="content">
            <h1>If you have any more questions, feel free to contact us!</h1>
            <p>We are still in stealth mode, so stay tuned...</p>
            <div class="subscribe-section">
                <div class="buttons">
                    <button class="social-media-btn twitter">
                        <div class="img"><img src="./../assets/images/Web/twitter.png" alt=""></div>
                        <p>TWITTER</p>
                    </button>
                    <button class="social-media-btn email">
                        <div class="img"><img src="./../assets/images/Web/email.png" alt=""></div>
                        <p>EMAIL</p>
                    </button>
                    <button class="social-media-btn youtube">
                        <div class="img"><img src="./../assets/images/Web/youtube.png" alt=""></div>
                        <p>YOUTUBE</p>
                    </button>
                </div>
                <div class="divider"></div>
                <div class="subscriber-button">
                    <div class="input" @click="focusInput">
                        <input type="email" placeholder="ENTER YOUR EMAIL" id="email">
                    </div>
                    <div class="subscribe">
                        <button>SUBSCRIBE</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'ContactUs', 
    methods:{
        focusInput(){
            document.getElementById('email').focus()
        }
    }
}
</script>

<style scoped>
    .content h1{
        font-size: 50px;
        font-weight:500;
        text-align: center;
    }
    .content p{
        font-size:20px;
        font-weight: bold;
        color:#191923;
        text-align: center;
        opacity:0.5;
        text-transform: uppercase;
        letter-spacing:5px;
        margin-top:30px;
    }
    .subscribe-section{
        margin-top:100px;
    }
    .buttons{
        display:flex;
        justify-content:space-between;
    }
    .social-media-btn{
        width:390px;
        height: 80px;
        border:none;
        border-radius:40px;
        display:flex;
        align-items: center;
    }
    .social-media-btn  p{
        margin:0px;
        opacity: 1;
        font-size:20px;
        font-weight:500;
        color:white;
        margin-left:80px;
    }
    .social-media-btn .img{
        margin-left:20px;
    }
    .twitter{
        background-color:#1DA1F2;
    }
    .email{
        background-color:#191923;
    }
    .email p{
        margin-left: 110px;
    }
    .youtube{
        background-color:#FF0000;
    }
    .divider{
        width:440px;
        margin: 50px auto;
        border-top:1px solid var(--main-text-color);
        opacity:0.2;
    }
    .subscriber-button{
        height: 80px;
        position: relative;
    }
    .input{
        width:1005px;
        border-radius: 40px;
        height:100%;
        background-color: #19192332;
        display:flex;
        align-items: center;
    }
    .input input{
        border:none;
        background-color:transparent;
        color:#191923;
        height:60px;
        font-size:20px;
        margin-left: 20px;
    }
    .input input:focus{
        outline:none;
        width:50%;
    }
    .subscribe{
        height:100%;
        position:absolute;
        top:0px;
        right:0px;
    }
    .subscribe button{
        width: 390px;
        height: 100%;
        border-radius: 40px;
        border:none;
        font-size:20px;
        letter-spacing: 5px;
        background-color:var(--primary-color);
    }
</style>