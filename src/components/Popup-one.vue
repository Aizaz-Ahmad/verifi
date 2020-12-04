<template>

    <div class="popup-backdrop"></div>
    <div class="popup-container">
        <div class="popup">
            <div class="close-popup"><span>&times;</span></div>
            <div class="header">
                <h1>AAVE Smart Contract On-Chain</h1>
            </div>
            <div class="features">
                <div class="feature">
                    <div class="feature-image">
                        <img src="./../assets/images/Web/Popup-File-Icon-Web.png" alt="">
                    </div>
                    <div class="feature-description">
                        <p class="header">Landing pools & Landing pool care</p>
                        <p class="description">Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy</p>
                    </div>
                    <div class="five-star">
                        <img src="./../assets/images/Web/Star.png" alt="">
                        <p>5.0</p>
                    </div>
                    <div class="button-btn">
                        <button>View Full Report</button>
                    </div>
                </div>
                <div class="feature">
                    <div class="feature-image">
                        <img src="./../assets/images/Web/Popup-File-Icon-Web.png" alt="">
                    </div>
                    <div class="feature-description">
                        <p class="header">Landing pools & Landing pool care</p>
                        <p class="description">Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy</p>
                    </div>
                    <div class="five-star">
                        <img src="./../assets/images/Web/Star.png" alt="">
                        <p>5.0</p>
                    </div>
                    <div class="button-btn">
                        <button>View Full Report</button>
                    </div>
                </div>
                <div class="feature">
                    <div class="feature-image">
                        <img src="./../assets/images/Web/Popup-File-Icon-Web.png" alt="">
                    </div>
                    <div class="feature-description">
                        <p class="header">Landing pools & Landing pool care</p>
                        <p class="description">Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy</p>
                    </div>
                    <div class="five-star">
                        <img src="./../assets/images/Web/Star.png" alt="">
                        <p>5.0</p>
                    </div>
                    <div class="button-btn">
                        <button>View Full Report</button>
                    </div>
                </div>
                <div class="feature">
                    <div class="feature-image">
                        <img src="./../assets/images/Web/Popup-File-Icon-Web.png" alt="">
                    </div>
                    <div class="feature-description">
                        <p class="header">Landing pools & Landing pool care</p>
                        <p class="description">Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy</p>
                    </div>
                    <div class="five-star">
                        <img src="./../assets/images/Web/Star.png" alt="">
                        <p>5.0</p>
                    </div>
                    <div class="button-btn">
                        <button>View Full Report</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name:'PopupOne',
    methods:{
        
    }
}
</script>
<style scoped>
    .popup{
        --popup-width:1000px;
        width:var(--popup-width);
        background-color:#F5F5F5;
        z-index: 1;
        position: absolute;
        margin-top:40px;
        border-radius: 30px;
   }
    .header{
        margin:30px 0px;
    }
    .header h1{
        font-size:30px;
        font-weight: bold;
        text-align: center;
    }
    .features{
        margin: 0 auto;
        margin-bottom: 20px;
        padding:0px 40px;
    }
    .feature{
        display:flex;
        padding:10px;
        margin-bottom: 20px;
        align-items: center;
        border-radius:10px;
        background-color:white;
    }
    .feature-image, .five-star{
        max-width:77px;
        max-height:77px;
        min-width:77px;
        min-height:77px;
        max-width:77px;
        max-height:77px;
        border-radius:10px;
        background-color:#19192332;
        display:flex;
        justify-content: center;
        align-items: center;
    }
    .feature-image img{
        width:50px;
        height:50px;
    }
    .feature-description{
        margin-left:20px;
    }
    .feature-description p.header{
        font-size:18px;
        margin:0px 0px 10px 0px;
        font-weight: bold;
    }
    .feature-description p.description{
        font-size:16px;
    }
    .five-star{
        background-color:var(--primary-color);
        margin-left:20px;
        flex-direction: column;
    }
    .five-star p{
        color:var(--main-text-color);
        font-size:24px;
        font-weight:bold;
    }
    .button-btn{
        display: flex;
        align-items: center;
        margin-left: 20px;
    }
    .button-btn button{
        width:188px;
        height: 51px;
        background-color:#19192332;
        border-radius:26px;
        border:none;
        cursor: pointer;
    }
    .close-popup{
        position: absolute;
        top:15px;
        right:15px;
        width:24px;
        height: 24px;
        background-color:#19192332;
        border-radius:30px;
        display:flex;
        align-items: center;
        justify-content:center;
        cursor: pointer;
    }
    .close-popup span{
        text-align: center;
        color:var(--main-text-color);
        font-size:24px;
    }
    @media screen and (max-width:1020px) {
        .popup{
            --popup-width:900px;
        }
    }
    @media screen and (max-width:920px) {
        .popup{
            --popup-width:800px;
        }
    }
    @media screen and (max-width:820px) {
        .popup{
            --popup-width:756px;
        }
    }
    @media screen and (max-width:780px) {
        
    }
</style>
