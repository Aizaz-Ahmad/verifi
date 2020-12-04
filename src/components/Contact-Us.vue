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
    .container{
        display:flex;
        justify-content:center;
        align-items:center;
        padding:0px;
    }
    .content h1{
        font-size: calc(50 / 1920 * 100vw);
        font-weight:500;
        text-align: center;
    }
    .content p{
        font-size:calc(20 / 1920 * 100vw);
        font-weight: bold;
        color:#191923;
        text-align: center;
        opacity:0.5;
        text-transform: uppercase;
        letter-spacing:calc(5 / 1920 * 100vw);
        margin-top:calc(30 / 1080 * 100vh);
    }
    .subscribe-section{
        margin-top:calc(100 / 1080 * 100vh);
    }
    .buttons{
        display:flex;
        justify-content:space-between;
    }
    .social-media-btn{
        width:calc(390 / 1920 * 100vw);
        height: calc(80 / 1080 * 100vh);
        border:none;
        border-radius:40px;
        display:flex;
        align-items: center;
    }
    .social-media-btn  p{
        margin:0px;
        opacity: 1;
        font-size:calc(20 / 1920 * 100vw);
        font-weight:500;
        color:white;
        margin-left:calc(80 / 1920 * 100vw);
    }
    .social-media-btn .img{
        margin-left:calc(20 / 1920 * 100vw);
    }
    .twitter{
        background-color:#1DA1F2;
    }
    .email{
        background-color:#191923;
    }
    .email p{
        margin-left: calc(110 / 1920 * 100vw);
    }
    .youtube{
        background-color:#FF0000;
    }
    .divider{
        width:calc(440 / 1920 * 100vw);
        margin: calc(50 / 1080 * 100vh) auto;
        border-top:1px solid var(--main-text-color);
        opacity:0.2;
    }
    .subscriber-button{
        height: calc(80 / 1080 * 100vh);
        position: relative;
    }
    .input{
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
        height:calc(60 / 1080 * 100vh);
        font-size:calc(20 / 1920 * 100vw);
        margin-left: calc(20 / 1920 * 100vw);
    }
    .input input:focus{
        outline:none;
    }
    .subscribe{
        height:100%;
        position:absolute;
        top:0px;
        right:0px;
    }
    .subscribe button{
        width: calc(390 / 1920 * 100vw);
        height: 100%;
        border-radius: 40px;
        border:none;
        font-size:calc(20 / 1920 * 100vw);
        letter-spacing: calc(5 / 1920 * 100vw);
        background-color:var(--primary-color);
    }
    @media screen  and (max-width: 768px){
        .container{
            /* display:block; */
             /* padding-top:calc(100 / var(--standard-mobile-height) * 100vh); */
        }
        .content{
            width: calc(335 / var(--standard-mobile-width) * 100vw);
        
        }
        .content h1{
            font-size: calc(30 / var(--standard-mobile-width) * 100vw);
            text-transform: capitalize;
            line-height: 1.5;
        }
        .content p {
            font-size:calc(16 / var(--standard-mobile-width) * 100vw);
        }
        .subscribe-section{
            margin-top: calc(50 / var(--standard-mobile-height) * 100vh);
        }
        .buttons{
            flex-direction: column;
        }
        .social-media-btn{
            width: calc(335 / var(--standard-mobile-width) * 100vw);
            height: calc(50 / var(--standard-mobile-height) * 100vh);
            margin-bottom: calc(20 / var(--standard-mobile-height) * 100vh);
        }
        .social-media-btn:last-of-type{
            margin-bottom: 0px;
        }
        .social-media-btn p{
            font-size: calc(16 / var(--standard-mobile-width) * 100vw);
            margin-left: calc(80 / var(--standard-mobile-width) * 100vw);
        }
        .social-media-btn .img{
            margin-left: calc(20 / var(--standard-mobile-width) * 100vw);
        }
        .social-media-btn .img img{
            width:35px;
            height:24px;
        }
        .social-media-btn.email img{
            width:24px;
        }
        .email p{
            margin-left: calc(100 / var(--standard-mobile-width) * 100vw);
        }
        .divider{
            width: calc(295 / var(--standard-mobile-width) * 100vw);
            margin: calc(40 / var(--standard-mobile-height) * 100vh) auto;
        }
        .subscriber-button{
            height:auto;
            width: calc(335 / var(--standard-mobile-width) * 100vw);
        }
        .input{
            margin-bottom: calc(20 / var(--standard-mobile-height) * 100vh);
            height: calc(50 / var(--standard-mobile-height) * 100vh);
        }
        .input input{
            width: 100%;
            font-size: calc(16 / var(--standard-mobile-width) * 100vw);
            height: calc(50 / var(--standard-mobile-height) * 100vh);
            text-align: center;
            margin-left: 0;
        }
        .subscribe{
            position: relative;
            width:100%;
        }
        .subscribe button{
            width:100%;
            height: calc(50 / var(--standard-mobile-height) * 100vh);
            font-size: calc(16 / var(--standard-mobile-width) * 100vw);
            letter-spacing: calc(5 / var(--standard-mobile-width) * 100vw);
        }
    }
</style>


