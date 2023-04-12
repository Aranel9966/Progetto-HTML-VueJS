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
    <div>
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
.container{
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    background-color: #ff4450;
    padding: 30px;
    .text{
        width: 700px;
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
        }
    }
}
.title{
    text-align: center;
    padding: 50px;
}
.btn{
    display: flex;
    justify-content: center;
    padding-bottom: 50px;
    .btn-primary{
        background-color: #ff4450;
        border-radius: 40px;
        padding: 15px 25px;
        border-color: transparent;
        color: white;
        margin: 20px 0;
    }
}

</style>