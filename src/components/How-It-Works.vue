<template>
    <div class="container">
        <div class="content">
            <h1 class="header">How it works</h1>
            <p class="description">Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum</p>
            <div class="features">
                <div class="feature">
                    <div class="img desktop-img"><img src="./../assets/images/Web/How-It-works-1.png" alt=""></div>
                    <div class="img mobile-img"><img src="./../assets/images/Web/HIW-1-Mobile.png" alt=""></div>
                    <div class="work-description">
                        <p>Pick a contract, which you want to analyze</p>
                    </div>
                </div>
                <div class="feature">
                    <div class="img desktop-img"><img src="./../assets/images/Web/How-It-works-2.png" alt=""></div>
                    <div class="img mobile-img"><img src="./../assets/images/Web/HIW-2-Mobile.png" alt=""></div>
                    <div class="work-description">
                        <p>Our sophisticated scanners will look for a bug</p>
                    </div>
                </div>
                <div class="feature">
                    <div class="img desktop-img"><img src="./../assets/images/Web/How-It-works-3.png" alt=""></div>
                    <div class="img mobile-img"><img src="./../assets/images/Web/HIW-3-Mobile.png" alt=""></div>
                    <div class="work-description">
                        <p>secure your earnings and make more money</p>
                    </div>
                </div>
            </div>
            <p class="description">Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum</p>
        </div>
    </div>
</template>

<script>
export default {
    name:'HowItWorks'
}
</script>

<style scoped>
    .container{
        background-color:var(--main-text-color);
    }
    .header{
        font-size: calc(50 / 1920 * 100vw);
        font-weight: 500;
        color:white;
        text-align: center;
    }
    p.description{
        font-size:calc(20 / 1920 * 100vw);
        opacity:0.6;
        font-weight: lighter;
        color:white;
        line-height: 1.6;
        margin: calc(50 / 1080 * 100vh) 0px;
    }
    .features{
        display:flex;
        justify-content:space-between;
        margin-top:calc(40 / 1080 * 100vh);
    }
    .features .feature{
        width:calc(360 / 1920 * 100vw);
        height:calc(271 / 1080 * 100vh);
        position:relative;
        border-radius:20px;
        overflow: hidden;
        display:flex;
        flex-direction: column;
        justify-content:center;
    }
    .features .feature:before{
        content:'';
        width:100%;
        height:100%;
        position:absolute;
        top:0px;
        left:0px;
        opacity:0.05;
        background-color:white;
    }
    .feature .work-description{
        width:calc(260 / 1920 * 100vw);
        margin:0 auto;
        margin-top:calc(30 / 1080 * 100vh);
    }
    .feature .work-description p{
        color:white;
        font-size:calc(20 / 1920 * 100vw);
        text-align: center;
        line-height:1.6;
    }
    .feature .img{
        text-align: center;
    }
    .desktop-img{
        display:block;
    }
    .mobile-img{
        display:none;
    }
    @media screen  and (max-width:768px){
        .desktop-img{
            display:none;
        }
        .mobile-img{
            display:block;
        }
        .content{
            width: calc(335 / var(--standard-mobile-width) * 100vw);
        }
        .header{
            font-size: calc(30 / var(--standard-mobile-width) * 100vw);
        }
        p.description{
            font-size: calc(14 / var(--standard-mobile-width) * 100vw);
            margin: calc(30 / var(--standard-mobile-height) * 100vh) 0px;
        }
        .features{
            flex-direction: column;
            margin-top: calc(40 / var(--standard-mobile-height) * 100vh);
        }
        .features .feature{
            width: 100%;
            height: calc(75 / var(--standard-mobile-height) * 100vh);
            margin-bottom: calc(20 / var(--standard-mobile-height) * 100vh);
            flex-direction: row;
            align-items: center;
        }
        .feature .work-description{
            margin-top:0px;
            width: auto;
        }
        .feature .work-description p{
            font-size: calc(16 / var(--standard-mobile-width) * 100vw);
            line-height: 1;
        }
        .feature .img{
            margin: 0px 5px;
        }
    }
</style>