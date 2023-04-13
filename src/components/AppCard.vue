<script>
import { store } from '../store';
export default {
    name:'AppCard',
    data(){
        return{
            store,
        }
    },
    props:{
        cards:Array,
    },
   
}
</script>
<template>
    <div class="row">
        
        <div v-for="(card,index) in cards"  v-show="card.text.toLowerCase().includes(this.store.search.toLowerCase())" class="card">
            <div class="img-card">
                <img :src=card.img alt="">
            </div>
            <div class="text-card">
                <span>{{card.type}} > </span>
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
.row{
    display: flex;
    flex-direction: row;
    justify-content: center;
    gap: 10px;
    padding: 50px;
    .card{
        background-color: white;
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
@media only screen and (max-width: 690px) {
  .row{
    flex-wrap: wrap;
  }
}
</style>