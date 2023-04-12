<script>
export default{
    name:'AppFooter',
  data(){
    return{

    }
  }
}
</script>
<template>
    <footer>
        <div class="footer-top">
            <div>
                <h3>ABOUT</h3>
                <p>
                    Sed nec felis pellentesquer lacinia dui sede
                    uttricies sapien. Pellentesque orci lectus,
                    consecteturvelr rutrum eu ipsum. Mauris
                    accurnsan eros eget libero posuere
                    vul putate.
                </p>
            </div>
            <div>
                <h3>CONTACT</h3>
                <p>USA Callifornia 20, First Avenue, Callifornia</p> <br>
                <p>Tel.:121245830032</p>
                <p>Fax.:121245830032</p> <br>
                <p><em> info@masterstudy.com</em></p>
            </div>
            <div>
                <h3>SOCIAL NETWORK</h3>
                <img class="social" src="../../public/images/Screenshot 2023-04-12 175324.png" alt="">
            </div>
            <div>
                <img src="../../public/images/Top-udemy-courses-90-percent-off.jpg" alt="">
            </div>
        </div >
        <hr>
        <div class="footer-bot">
            <img src="../../public/images/footer-logo2x-50x56.png" alt="">
            <span>copyright@ 2020. Maste6tudy Theme by SMemmemes</span> 
        </div>
    </footer>
</template>
<style lang="scss" scoped>
footer{
    background-color: #273044;
    color: white;
    .footer-top{
        display: flex;
        justify-content: center;
        gap: 120px;
        padding: 30px;
        div{
            width: 200px;
            h3{
                padding-bottom: 15px;
            }
        img{
            height: 150px;
        }
        .social{
            margin-left: -35px;
        }
        }
        
    }
    .footer-bot{
        display: flex;
        align-items: center;
        gap: 20px;
        width: 1200px;
        margin: auto;
        padding: 20px;
        img{
            width: 30px;
        }
    }
}

</style>