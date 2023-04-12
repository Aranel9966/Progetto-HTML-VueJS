<script>
export default {
    data(){
        return{

        }
    }
}
</script>
<template>
    <div>
        <div class="jumbotron-bar">
            <ul>
                <li><span><i class="fa-solid fa-chart-column"></i></span> <a href=""> Busness</a></li>
                <li><span><i class="fa-solid fa-palette"></i></span> <a href=""> Design</a></li>
                <li><span><i class="fa-solid fa-gear"></i></span> <a href=""> Development</a></li>
                <li><span><i class="fa-regular fa-face-smile"></i></span> <a href=""> Lifestyle</a></li>
                <li><span><i class="fa-solid fa-wallet"></i></span> <a href=""> Office Productivity</a></li>
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
        a{
        text-decoration: none;
        color: white;
        }
        display: flex;
        flex-direction: row;
        gap: 40px;
        list-style-type: none;
        span{
            padding: 10px;
        }
    }
}
.jumbotron{
    display: flex;
    flex-direction: row;
    width: 100%;
    position: relative;
    justify-content: flex-end;
    margin-bottom: 100px;
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