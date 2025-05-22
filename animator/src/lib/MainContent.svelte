<script>
    export let animationClass;
    export let animationStyle;
    export let applyAnimation;
</script>

<div class="main">
    <div class="mainHead">
        <div class="zoomBtn">
            <div class="zoom">
                <img src="../assets/Heart.svg" alt="">
            </div>
            <div class="zoom">
                <img src="/reload.svg" alt="">
            </div>
        
        </div>
        <div class="exportBtn">
            <button class="pBtn">export</button>
        </div>
    </div>
    <div class="mainBody">
        <div class="animationBox">
            <div class="swiper-container">
                <button class="btn" on:click={() => applyAnimation("rotate")}>Rotations</button>
                <button class="btn" on:click={() => applyAnimation("rotate2")}>Rotations 2</button>
                <button class="btn" on:click={() => applyAnimation("flip")}>Flip</button>
                <button class="btn" on:click={() => applyAnimation("flip2")}>Flip 2</button>
                <button class="btn" on:click={() => applyAnimation("slide")}>Slide</button>
                <button class="btn" on:click={() => applyAnimation("slide2")}>Slide 2</button>
            </div>
        </div>
        <div class="objectSquare">

        </div>
    </div>
    
</div>

<!-- <div class="main">
    <div class="box">
        <button class="btn" on:click={() => applyAnimation("rotate")}>Rotations</button>
        <button class="btn" on:click={() => applyAnimation("rotate2")}>Rotations 2</button>
        <button class="btn" on:click={() => applyAnimation("flip")}>Flip</button>
        <button class="btn" on:click={() => applyAnimation("flip2")}>Flip 2</button>
        <button class="btn" on:click={() => applyAnimation("slide")}>Slide</button>
        <button class="btn" on:click={() => applyAnimation("slide2")}>Slide 2</button>
    </div>
    <div class="main-content">
        <div class="object {animationClass}" style={animationStyle}></div>
    </div>
</div> -->

<!-- <style>
    .btn{
        width: max-content;
        height: 35px;
        margin: 0px 0px;
        padding: 0px 5px;
    }
    .box{
        position: absolute;
        margin: 5vh 25vw;
        border: 2px solid black;
        padding: 20px;
        display: flex;
        gap: 20px;
        background: #a99f9f87;
        border-radius: 20px;
    }
    .main{
        display: flex;
        flex-direction: column;
        width: 100%;
        gap: 20px;
        /* height: auto; */
    }
    .main-content {
        padding: 20px;
        flex-grow: 1;
        display: flex;
        justify-content: center;
        align-items: center;
        background: #e5e1e1;
    }
    .object {
        width: 100px;
        height: 100px;
        background-color: #4c5273;
    }
</style> -->

<style>
    .main {
        width: 100%;
        height: 100%;
        max-height: 100%;
        background-size: auto, auto, auto;
        background-size: 30px 30px;
        display: flex;
        flex-direction: column;
        position: relative;
        z-index: 500;
    }
    .mainHead {
        display: flex;
        padding: 30px;
        justify-content: space-between;
    }
    .mainBody {
        display: flex;
        justify-content: center;
        /* align-items: center; */
        height: 100%;
        width: 100%;
        position: relative;
    }
    .animationBox {
        background-color: #fff !important;
        height: 90px;
        min-width: 400px;
        max-width: 900px;
        border-radius: 10px;
        box-shadow: -2px 3px 12px -5px #e2e2e2;
        display: flex;
        
        align-items: center;
        /* justify-content: center; */
        position: relative;
        z-index: 1000;
        border: 4px solid black;
    }
    .swiper-container {
        display: flex;
        gap: 4px;
        margin-left: auto;
        margin-right: auto;
        position: relative;
        overflow: hidden;
        list-style: none;
        padding: 0;
        z-index: -1;
    }
    .btn{
        width: max-content;
        height: 40px;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: #d6d4de;
        font-family: "Poppins";
        color: #282828;
        font-weight: 600;
        border-radius: 10px;
        cursor: pointer;
        font-size: 14px;
        padding: 0 20px;
        position: relative
    }
    .objectSquare{
        margin-top: 200px;
        position: absolute;
        width: 150px;
        height: 150px;
        background-color: #ffa5a5;
        border-radius: 10px;
    }
    .zoomBtn{
        display: flex;
    }
    .zoom{
        width: 40px;
        height: 40px;
        border-radius: 20px;
        background-color: #fff;
        margin-right: 5px;
        box-shadow: 0 3px 8px 0 #c7c7c7;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 22px;
        font-family: "Poppins";
        font-weight: 700;
        color: #9893aa;
        cursor: pointer
    }
    .pBtn{
        font-family: "Poppins";
        background-color: midnightblue;
        color: #fff;
        font-weight: 700;
        padding: 10px 40px;
        border-radius: 7px;
        cursor: pointer;
        text-decoration: none;
    }
</style>
