<script>
import AppHeader from './components/AppHeader.vue';
import '@fortawesome/fontawesome-free/css/all.css';
import AppjumbotronVue from './components/Appjumbotron.vue';
import AppCard from './components/AppCard.vue';
import AppMainTop from './components/AppMainTop.vue';
import AppMainMid from './components/AppMainMid.vue';
import AppMainBot from './components/AppMainBot.vue';
export default{
  data(){
    return{
      cards1:[
                {
                    type:'Decelopment',
                    img:"../../public/images/895786_7b4b_2-272x161.jpg" ,
                    text:'The Complete iOS 10 & Swift 3 Developer Course',
                    vote:4,
                    price:'$199.99',
                    discount:'$100'
                },
                {
                    type:'Decelopment',
                    img:"../../public/images/246154_d8b0_3-272x161.jpg" ,
                    text:'Web Design for Beginners: Real World coding in HTML & CSS',
                    vote:4,
                    price:'$129.99',
                    discount:'$64'
                },
                {
                    type:'Decelopment',
                    img:"../../public/images/752950_b773-272x161.jpg" ,
                    text:'GitHub Ultimate: Master Git and GitHub - Beginner to Expert',
                    vote:4,
                    price:'$99.99',
                    discount:'$50'
                },
                {
                    type:'Decelopment',
                    img:"../../public/images/1253188_58f7_2-272x161.jpg" ,
                    text:'The complete iOS 11 & Swift Developer Course - Build 20 Apps',
                    vote:4,
                    price:'$199.99',
                    discount:'$100'
                },
                {
                    type:'Decelopment',
                    img:"../../public/images/919872_ed54_6-272x161.jpg" ,
                    text:'Android Java Masterclass - Become an App Developer',
                    vote:4,
                    price:'$99.99',
                    discount:'$50'
                },
                {
                    type:'Decelopment',
                    img:"../../public/images/951684_9c1a_2-272x161.jpg" ,
                    text:'Xamarin Forms: Build Native Cross•platform Apps with C#',
                    vote:4,
                    price:'$109.99',
                    discount:'$95'
                },
      ],
      cards2:[
                {
                    type:'Decelopment',
                    img:"../public/images/895786_7b4b_2-272x161.jpg" ,
                    text:'The Complete iOS 10 & Swift 3 Developer Course',
                    vote:4,
                    price:'$199.99',
                    discount:'$100'
                },
                
                {
                    type:'Design',
                    img:"../public/images/1561458_7f3b-272x161.jpg " ,
                    text:'CSS - The Complete Guide 2020 (incl. Flexbox, Grid & Sass)',
                    vote:5,
                    price:'$199.99',
                    discount:'$100'
                },
                {
                    type:'Decelopment',
                    img:"../public/images/246154_d8b0_3-272x161.jpg" ,
                    text:'Web Design for Beginners: Real World coding in HTML & CSS',
                    vote:4,
                    price:'$129.99',
                    discount:'$65'
                },
                {
                    type:'Design',
                    img:"../public/images/1208228_d61c_4-272x161.jpg" ,
                    text:'Digitally Painting Light and Colar: Amateur to Master',
                    vote:4,
                    price:'$139.99',
                    discount:'$70'
                },
                {
                    type:'Arts & Crafts',
                    img:"../public/images/186792_41e4_4-272x161.jpg" ,
                    text:'Become an Arabic Calligraphy Artist from Scratch',
                    vote:4,
                    price:'',
                    discount:'$199.99'
                },
                {
                    type:'Google',
                    img:"../public/images/1776542_30b1-272x161.jpg" ,
                    text:'Google Searching Ninja!',
                    vote:4,
                    price:'$89.99',
                    discount:'$45'
                },
      ],
      cards3:[
                {
                    type:'Arts & Crafts',
                    img:"../public/images/949316_2a64_11-272x161.jpg" ,
                    text:'Foundations for Mastering Watercolor Painting',
                    vote:4,
                    price:'$19.99',
                    discount:'$10'
                },
                
                {
                    type:'Food & Beverage',
                    img:"../public/images/366802_6fcc-272x161.jpg" ,
                    text:'Get Wine-Smart',
                    vote:4,
                    price:'$49.99',
                    discount:'$25'
                },
                {
                    type:'Arts & Crafts',
                    img:"../public/images/381588_2e6d_4-272x161.jpg" ,
                    text:'The Colored Pencil Drawing Course',
                    vote:4,
                    price:'$34.99',
                    discount:'$18'
                },
                {
                    type:'Arts & Crafts',
                    img:"../public/images/838056_611a_3-272x161.jpg" ,
                    text:'Paint Realistic Watercolor and Botanicals - STUDIO BASICS',
                    vote:4,
                    price:'$69.99',
                    discount:'$35'
                },
                {
                    type:'Arts & Crafts',
                    img:"../public/images/1414956_d944_15-272x161.jpg" ,
                    text:'Mastering Brushstrokes - Part 1',
                    vote:4,
                    price:'$19.99',
                    discount:'$10.99'
                },
                {
                    type:'Arts & Crafts',
                    img:"../public/images/1109398_4c13-272x161.jpg ",
                    text:'Paint Realistic Watercolour and Botanicals - MAGNOLIAS',
                    vote:4,
                    price:'$69.99',
                    discount:'$35'
                },
      ]
    }
  },
  components:{
    AppHeader,
    AppjumbotronVue,
    AppCard,
    AppMainTop,
    AppMainMid,
    AppMainBot
  }
}
</script>

<template>
  <div>
    <AppHeader></AppHeader>
    <AppjumbotronVue></AppjumbotronVue>
    <AppCard :cards="cards1"></AppCard>
    <AppMainTop></AppMainTop>
    <AppCard :cards="cards2"></AppCard>
    <AppCard :cards="cards3"></AppCard>
    <AppMainMid></AppMainMid>
    <AppCard :cards="cards2" class="bg-color"></AppCard>
    <AppMainBot></AppMainBot>

  </div>
</template>

<style lang="scss" scoped>
.bg-color{
  background-color: #f0f4fa;
}
</style>
