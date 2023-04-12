<script>
export default {
    name:'AppMainTop',
    data(){
        return{

        }
    } 
}           
</script>
<template>
    <div class="bg-main">
        <div class="text">
            <h1>
                Limitless learning,
                more possibilities
            </h1>
            <p>
                Online courses open the opportunity for learning to almost anyone.
                regardless of their scheduling commitments.
            </p>
            <button class="btn-primary">READ MORE</button>
        </div>
    </div>
    <div class="main-menu">
        <h1>Recent courses</h1>
        <div class="menu">
            <ul>
                <li> <a href="#"> All Categories</a></li>
                <li> <a href="#"> Business</a></li>
                <li> <a href="#"> Design</a></li>
                <li> <a href="#"> Development</a></li>
                <li> <a href="#"> IT & Softwere</a></li>
                <li> <a href="#">  Lifestyle</a></li>
                <li> <a href="#"> Marketing</a></li>
                <li> <a href="#"> Office Productivity</a></li>
            </ul>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.bg-main{
    background-image: url('../../public/images/bg.png');
    height: 550px;
    width: 100%;
    position: relative;
    margin-bottom: 50px;
    .text{
        position: absolute;
        top: 40%;
        left: 20%;
        width: 450px;
        h1{
            font-size: 40px;
            padding-bottom: 10px;
        }
        // button{
        //     background-color: #ff4450;
        //     border-radius: 40px;
        //     padding: 15px 25px;
        //     border-color: transparent;
        //     color: white;
        //     margin: 20px 0;
        // }
    }
}
.main-menu{
    text-align: center;
    height: 130px;
    .menu{
        ul{
            justify-content: center;
            margin: 50px;
            gap: 25px;
            a:hover{
                background-color: #f0f4fa;
                color: rgb(131, 129, 129);
                border-radius: 20px;
                padding: 3px 10px;
            }
        }
        
    }
}
</style>