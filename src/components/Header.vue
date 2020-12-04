<template>
    <div class="container">
        <div class="logo">
            <svg xmlns="http://www.w3.org/2000/svg" width="80" height="40" viewBox="0 0 80 40">
                <text transform="translate(0 32)" fill="#fff" font-size="30" font-family="SegoeUI-Light, Segoe UI" font-weight="300"><tspan x="0" y="0">LO</tspan><tspan  y="0" fill="#32e875" font-family="SegoeUI-Bold, Segoe UI" font-weight="700">GO</tspan></text>
            </svg>
        </div>
        <div class="header-content">
            <div class="header-text-content animate__animated animate__fadeInLeft">
                <div class="investments">
                    <h1>DeFi INVESTMENTS</h1>
                </div>
                <h1 class="peace-of-mind">WITH PEACE OF MIND</h1>
                <p class="details">Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea</p>
                <p class="victim">Don’t be the victim of the next DAO hack.</p>
                <a href="#second-section" class="check-your-risk">
                    <div class="img"><img src="./../assets/images/Web/Check-Your-Risk-Icon.png" alt=""></div>
                        <p>CHECK YOUR RISK</p>
                    </a>
            </div>
            <div class="header-image  animate__animated animate__fadeInRight"></div>
        </div>
        <div class="arrow animate__animated animate__heartBeat animate__slow animate__infinite">
            <img src="./../assets/images/Web/Arrow.png" alt="">
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
    .container {
        padding:0px;
        background-color:var(--main-text-color);
        position: relative;
    }
    .logo{
        position:absolute;
        top:30px;
        left: 10.42vw;
    }
    .arrow{
        position:absolute;
        bottom: 20px;
        left: 0px;
        width:100%;
        text-align: center;
    }
    .header-content{
        width:100%;
        height:100%;
        display:grid;
        grid-template-columns: calc(200 / 1920 * 100vw) calc(623 / 1920 * 100vw) auto;
    }
    .header-content .header-image{
        grid-area: 1 / 3;
        background-image:url('./../assets/images/Web/Header-Image.png');
        background-repeat: no-repeat;
        background-size:100% 100%;
    }
    .header-content .header-text-content{
        grid-area: 1 / 2 / 1 / 3;
    }
    .investments{
        background-color:white;
        width:calc(557 / 1920 * 100vw);
        height:calc(112 / 1080 * 100vh);
        margin-top:18.24vh;
        display:flex;
        align-items: center;
        justify-content:center;
    }
    .investments h1{
        font-size:calc(60 / 1920 * 100vw);
        font-weight:bold;
        color:#24126A;
    }
    .peace-of-mind{
        margin-top:10px;
        font-size: calc(50 / 1920 * 100vw);
        font-weight: 500;
        color:white;
        letter-spacing:calc(5 / 1920 * 100vw);
    }
    .details{
        width: calc(557 / 1920 * 100vw);;
        font-size: calc(20 / 1920 * 100vw);
        font-weight:300;
        color:white;
        opacity: 0.5;
        line-height: 1.7;
        margin-top: 9.26vh;
    }
    .victim{
        margin-top:3.7vh;
        font-size:calc(20 / 1920 * 100vw);
        font-weight:bold;
        color:var(--primary-color);
        text-transform: uppercase;
        letter-spacing: calc(5 / 1920 * 100vw);
    }
    .check-your-risk{
        width:calc(329 / 1920 * 100vw);
        height:calc(70 / 1080 * 100vh);
        background-color:var(--primary-color);
        border-radius: 35px;
        border: none;
        display:flex;
        align-items: center;
        margin-top:12.03vh;
    }
    .check-your-risk .img{
        margin-left: calc(20 / 1920 * 100vw);;
    }
    .check-your-risk p{
        font-size: calc(20 / 1920 * 100vw);
        font-weight:500;
        margin-left:calc(50 / 1920 * 100vw);
    }
</style>