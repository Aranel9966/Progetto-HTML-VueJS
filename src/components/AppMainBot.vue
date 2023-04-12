<script>
export default {
    name:'AppMainBot',
    data(){
        return{

        }
    },
}  
</script>
<template>
    <div class="container-top">
        <div class="left">
            <i class="fa-solid fa-chevron-left"></i>
        </div>
        <div class="right">
            <i class="fa-solid fa-chevron-right"></i>
        </div>
    </div>
    <div class="container">

        <div class="left-container">
            <div class="img">
                <img src="../../public/images/image_box_1-221x231.png" alt="">
            </div>
            <div class="text-container">
                <h2>Become an Instructor</h2>
                <p>Teach what you love. Masters:udy gives the tools to create a course. </p>
                <button class="btn-primary">START TEACHING</button>
            </div>
        </div>
        <div class="right-container">
            <div class="img">
                <img src="../../public/images/image_box_2-234x231.png" alt="">
            </div>
            <div class="text-container">
                <h2>Access For Business</h2>
                <p>Get unlimited access to 2,500 of top courses for your team. </p>
                <button class="btn-primary">DOING BUSINESS</button>
            </div>
    
        </div>
    </div>
    <div class="container-bot">
        <div class="text">
            <h2>Investing for Your Future</h2>
            <p>
                lt iS no exaggeraton to say thiS MasterStudy experience was
                transformetive-both professionelly and personelly. ThiS workshop
                will long remain a high point of my life. Thanks again..., I arn feeling
                energized and eager to start teaching my class next week. I cant wait
                to use all of my new teaching tools. I Will absolutely recommend thiS
                workshop to Other educatorsl
            </p>
            <p>
                <strong>Linda Green</strong> <br>
                <em>Product Manager, Apple Inc</em>
            </p>
        </div>
    </div>


</template>
<style lang="scss" scoped>
.container-top{
    display: flex;
    flex-direction: row;
    justify-content: center;
    background-color: #f0f4fa;
    padding: 40px;
    .left,.right{
        padding:3px 8px;
        border: 1px solid lightgray;
        background-color: white;
        color:lightgray ;
    }
}
.container{
    display: flex;
    flex-direction: row;
    justify-content: center;
    padding: 40px;
    
    .left-container,.right-container {
        border: 1px solid lightgray;
        display: flex;
        align-items: center;
        margin: 10px;
        padding: 20px;
        .img{
            img{
                border-radius: 50%;
            }
        }
        .text-container{
            width: 400px;
            padding: 50px;
            p{
                color: gray;
            }
        }
        
    }
}
.container-bot{
    background-image: url('../../public/images/testimonial-1-1917x640-1-1914x639.jpg');
    height: 600px;
    position: relative;
    .text{
        line-height:32px;
        height: 450px;
        width: 600px;
        background-color: white;
        position: absolute;
        left: 500px;
        top: 100px;
        padding: 50px;
        display: flex;
        flex-direction: column;
        gap: 20px;
    }
}
</style>