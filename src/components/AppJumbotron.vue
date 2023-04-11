<script>
export default {
    date(){
        return{

        }
    }
}
</script>
<template>
    <div>
        <div class="jumbotron-bar">
            <ul>
                <li><span><i class="fa-solid fa-chart-column"></i></span>Busness</li>
                <li><span><i class="fa-solid fa-palette"></i></span>Design</li>
                <li><span><i class="fa-solid fa-gear"></i></span>Development</li>
                <li><span><i class="fa-regular fa-face-smile"></i></span>Lifestyle</li>
                <li><span><i class="fa-solid fa-wallet"></i></span>Office Productivity</li>
            </ul>
        </div>
        <div class="jumbotron">
            <div class="color">
                <div class="text">

                    <h1>Udemy Affiliate Sales</h1>
                    <p>Monetize your audience and attract new customers with Udemy!</p>
                </div>
            </div>
            <div class="img">
                <img src="../../public/images/slide-1.jpg" alt=""> 
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.jumbotron-bar{
    background-color: #273044;
    color: white;
    display: flex;
    justify-content: center;
    padding: 15px;
    margin-bottom: 20px;
    ul{
        display: flex;
        flex-direction: row;
        gap: 15px;
        list-style-type: none;
        span{
            padding: 5px;
        }
    }
}
.jumbotron{
    display: flex;
    flex-direction: row;
    width: 100%;
    position: relative;
    justify-content: flex-end;
    .color{
        width: 60%;
        border-right: 200px solid transparent;
        border-bottom: 325px solid #ff4450;
        position: absolute;
        top: 0;
        left: 0;
        .text{
            color: white;
            position: absolute;
            top: 100px;
            left:120px;
            overflow: auto;
        }
    }
    .img{
        display: flex;
        justify-content: flex-end;
        img{
            width: 800px;
        }
    }
}
</style>r