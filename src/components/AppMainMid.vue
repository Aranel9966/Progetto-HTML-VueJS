<script>
export default {
    name:'AppMainMid',
    data(){
        return{

        }
    } 
}           
</script>
<template>
    <div class="box">
        <div class="lateral-menu">
            <i class="fa-solid fa-tv"></i>
            <i class="fa-regular fa-circle-xmark"></i>
            <i class="fa-solid fa-wrench"></i>
            <i class="fa-solid fa-cart-shopping"></i>
            <i class="fa-solid fa-mobile-screen"></i>
        </div>
        <div class="btn">
            <button class="btn-primary">SHOW ALL</button>
        </div>
        <div class="container">
            <div class="text">
                <h2>
                    Subscribe our newsletter
                </h2>
                <p>
                    There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words
                </p> 
            </div>
            <div class="form">
                <p>YOUR E-MAIL ADDRESS</p> 
                <input type="text" placeholder="Enter Your E-mail">
                <button>SUBSCRIBE</button>
            </div>
        </div>
        <div class="title">
            <h1>Popular courses</h1>
            <div>Discover Our most popular courses for self learning</div>   
        </div>
    </div>
</template>
<style lang="scss" scoped>
.box{
    position: relative;

    .lateral-menu{
        position: absolute;
        padding: 10px;
        right: 0;
        top: -150px;
        display: flex;
        flex-direction: column;
        font-size: 25px;
        align-items: center;
        gap: 15px;
        border: 1px solid lightgray;
        box-shadow: 10px 10px 5px #dedede;
        color: rgb(62, 61, 61);
        i:hover{
            cursor: pointer;
            color: black;
        }
    }
    .container{
        display: flex;
        justify-content: center;
        align-items: center;
        color: white;
        background-color: #ff4450;
        padding: 30px;
        .text{
            max-width: 700px;
        }
        .form{
            input{
                margin: 10px 0;
                padding: 5px;
            }
            button{
                background-color: #457993;
                color: white;
                padding: 5px;
                border-color: transparent;
                border-radius: 0px;
            }
        }
    }
    .title{
        text-align: center;
        padding: 50px;
        background-color: #f0f4fa;
    }
    .btn{
        display: flex;
        justify-content: center;
        padding-bottom: 50px;
    }
}
</style>