<script>
export default {
    name:'AppMainTop',
    data(){
        return{
            options:[
                'All Categories',
                'Business',
                'Design',
                'Development',
                'IT & Softwere',
                'Lifestyle',
                'Marketing',
                'Office Productivity',
            ]
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
            <ul><li v-for="option in options"> <a href="#" > {{option}}</a></li></ul>
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
        max-width: 450px;
        h1{
            font-size: 40px;
            padding-bottom: 10px;
        }
    }
}
.main-menu{
    text-align: center;
    height: 130px;
    .menu{
        ul{
            flex-wrap: wrap;
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