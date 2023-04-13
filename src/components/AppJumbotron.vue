<script>
export default {
    data(){
        return{
            options:[
                {
                    option:'Busness',
                    icon:'fa-solid fa-chart-column'
                },
                {
                    option:'Design',
                    icon:'fa-solid fa-palette'
                },
                {
                    option:'Development',
                    icon:'fa-solid fa-gear'
                },
                {
                    option:'Lifestyle',
                    icon:'fa-regular fa-face-smile'
                },
                {
                    option:'Office Productivity',
                    icon:'fa-solid fa-wallet'
                }
            ]

        }
    }
}
</script>
<template>
    <div>
        <div class="jumbotron-bar">
            <ul>
                <li  v-for="option in options"><span><i :class=option.icon></i></span> <a href=""> {{option.option}}</a></li>
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
        <h2>Popular Development Courses</h2>
    </div>
</template>
<style lang="scss" scoped>
h2{
    margin-left: 105px;
}
.jumbotron-bar{
    background-color: #273044;
    color: white;
    display: flex;
    justify-content: center;
    padding: 15px;
    margin-bottom: 20px;
    ul{
        display: flex;
        flex-wrap: wrap;
        flex-direction: row;
        gap: 40px;
        list-style-type: none;
        a{
        text-decoration: none;
        color: white;
        }
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
        border-bottom: 398px solid #ff4450;
        position: absolute;
        top: 0;
        left: 0;
        .text{
            max-width: 400px;
            color: white;
            position: absolute;
            top: 100px;
            right:10%;
        }
    }
    .img{
        display: flex;
        justify-content: flex-end;
        img{
            max-width: 1000px;
        }
    }
}
</style>r