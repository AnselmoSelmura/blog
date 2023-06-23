<template>
        <section class="slider">
        <div class="slide-content">
            <input type="radio" name="btn-radio" id="radio1">
            <input type="radio" name="btn-radio" id="radio2">
            <input type="radio" name="btn-radio" id="radio3">
    
            <div class="slide-box primeiro">
                <img class="img-desctop" src="../assets/slid/slids (1).png" alt="">
                <img class="img-mobale" src="../assets/slid/slid/slide-mobale.png" alt="">
            </div>
            <div class="slide-box">
                <img class="img-desctop" src="../assets/slid/slids (2).png" alt="">
                <img class="img-mobale" src="../assets/slid/slid/slide-mobale1.png" alt="">
            </div>
            <div class="slide-box">            
                <img class="img-desctop" src="../assets/slid/slids (1).png" alt="">
                <img class="img-mobale" src="../assets/slid/slid/slide-mobale.png" alt="">
            </div>
            <!--Navegação-->
            <div class="nav-auto">
                <div class="auto-btn1"></div>
                <div class="auto-btn2"></div>
                <div class="auto-btn3"></div>
            </div>
            <div class="nav-manual">
                <label for="radio1" class="manual-btn"></label>
                <label for="radio2" class="manual-btn"></label>
                <label for="radio3" class="manual-btn"></label>
            </div>
        </div>
    </section>
</template>

<script>
    export default{
        name: 'carousel'
    }
</script>

<style>
    section.slider{
    overflow: hidden;
    margin: 0 auto;
    width: 100%;
    height: auto;
    padding: 0 !important;
    }
    .slide-content{
        width: 400%;
        height: auto;
        display: flex;
    }
    .slide-content input, .img-mobale{
        display: none;
    }
    .slide-box{
        width: 25%;
        height: auto;
        position: relative;
        text-align: center;
    }.slide-box img{
        width: 100%;
    }

    .nav-manual, .nav-auto{
        position: absolute;
        width: 100%;
        margin-top: 20%;
        display: flex;
        justify-content: center;
    }.nav-manual .manual-btn, .nav-auto div{
        border-radius: 50%; 
        border: 1px solid #ef0a0a;
        padding: 5px;
        cursor: pointer;
        transition: 1s;
    }
    .nav-manual .manual-btn:not(:last-child), .nav-auto div:not(:last-child){
        margin-right: 10px;
    }
    .nav-manual .manual-btn:hover{
        transition: all 1s;
        transform: scale(1.5);
        background-color: #ef0a0a;
    }

    #radio1:checked ~ .nav-auto .auto-btn1, #radio2:checked ~ .nav-auto .auto-btn2, #radio3:checked ~ .nav-auto .auto-btn3{
        background-color: #ef0a0a;
    }
    #radio1:checked ~ .primeiro{
        margin-left: 0%;
    }
    #radio2:checked ~ .primeiro{
        margin-left: -25%;
    }
    #radio3:checked ~ .primeiro{
        margin-left: -50%;
    }
</style>