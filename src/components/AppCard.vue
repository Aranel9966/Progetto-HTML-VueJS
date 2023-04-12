<script>
export default {
    name:'AppCard',
    data(){
        return{

            cards:[
                {
                    img:"../../public/images/895786_7b4b_2-272x161.jpg" ,
                    text:'The Complete iOS 10 & Swift 3 Developer Course',
                    vote:4,
                    price:'$199.99',
                    discount:'$100'
                },
                {
                    img:"../../public/images/246154_d8b0_3-272x161.jpg" ,
                    text:'Web Design for Beginners: Real World coding in HTML & CSS',
                    vote:4,
                    price:'$129.99',
                    discount:'$64'
                },
                {
                    img:"../../public/images/752950_b773-272x161.jpg" ,
                    text:'GitHub Ultimate: Master Git and GitHub - Beginner to Expert',
                    vote:4,
                    price:'$99.99',
                    discount:'$50'
                },
                {
                    img:"../../public/images/1253188_58f7_2-272x161.jpg" ,
                    text:'The complete iOS 11 & Swift Developer Course - Build 20 Apps',
                    vote:4,
                    price:'$199.99',
                    discount:'$100'
                },
                {
                    img:"../../public/images/919872_ed54_6-272x161.jpg" ,
                    text:'Android Java Masterclass - Become an App Developer',
                    vote:4,
                    price:'$99.99',
                    discount:'$50'
                },
                {
                    img:"../../public/images/951684_9c1a_2-272x161.jpg" ,
                    text:'Xamarin Forms: Build Native Cross•platform Apps with C#',
                    vote:4,
                    price:'$109.99',
                    discount:'$95'
                },
            ],
        }
    },
    methods: {
        search(){
            console.log(this.cards)
        }
    },
}
</script>
<template>
    <h2>Popular Development Courses</h2>
    <div class="row">
        <div v-for="(card,index) in cards" class="card">
            <div class="img-card">
                <img :src=card.img alt="">
            </div>
            <div class="text-card">
                <span>Development > </span>
                <p>{{ card.text }}</p>
                <hr>
                <div class="text-card-bot">
                    <div class="vote">
                        <img v-for="star in this.cards[index].vote " src="../../public/images/starfull.svg" ><img v-for="star in 5 - this.cards[index].vote " src="../../public/images/staremptyl.svg" >
                    </div>
                    <div class="price">
                        <span>
                            {{card.price}}
                        </span> 
                        <p>
                            {{card.discount}}
                        </p> 
                    </div>
                </div>
            </div>
        </div>

    </div>
</template>
<style lang="scss" scoped>
h2{
    margin-left: 105px;
}
.row{
    display: flex;
    flex-direction: row;
    justify-content: center;
    gap: 10px;
    padding: 50px;
    .card{
        border: 2px solid lightgray;
        width: 274px;
        .img-card{
            img{
                width:100%;
            }
        }
        .text-card{
            padding: 10px;
            span{
                color: lightgray;
            }
            hr{
                margin: 10px;
            }
            .text-card-bot{
                display: flex;
                justify-content: space-between;
                span{
                    text-decoration:line-through;
                }
            }
        }
    }

}
</style>