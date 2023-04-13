<script>
import { store } from '../store';

export default{
  data(){
    return{
      store,
    }
  }
}
</script>

<template>
  <div>
    <nav>
      <div class="nav-top">
        <p>English <span><i class="fa-solid fa-chevron-down"></i></span></p>
        <ul>
          <li>Home</li>
          <li>Pages</li>
          <li>Course Formats</li>
          <li>Demos</li>
          <li><i class="fa-brands fa-facebook"></i></li>
          <li><i class="fa-brands fa-twitter"></i></li>
          <li><i class="fa-brands fa-instagram"></i></li>
          <li><i class="fa-brands fa-linkedin"></i></li>
          <li><i class="fa-brands fa-google-plus-g"></i></li>
          <li><i class="fa-brands fa-youtube"></i></li>
        </ul>
      </div>
      <hr>
      <div class="nav-bot">
        <img src="../../public/images/MasterStudy.svg" alt="">
        <p><i class="fa-solid fa-bars"></i> CATEGORY</p>
        <div>
          <input v-model="store.search" type="text" placeholder="Search courses">
          <button class="btn"><i class="fa-solid fa-magnifying-glass"></i></button>
        </div>
        <a href="#"><span><i class="fa-solid fa-bullhorn"></i></span> Become an instructor</a>
        <a href="#"><span><i class="fa-solid fa-suitcase"></i></span> For Enterprise</a>
        <a href="#"><span><i class="fa-regular fa-user"></i></span> Log in</a>
        <button class="btn-primary">SING UP</button>
        <a href="#"><span><i class="fa-regular fa-bookmark"></i></span></a>
        
      </div>
    </nav>
  </div>
</template>

<style lang="scss" scoped>
nav{
  .nav-top{
    max-width: 1300px;
    margin: auto;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 10px;
    color: lightgrey;
    ul{
      list-style-type: none;
      display: flex;
      flex-wrap: wrap;
      flex-direction: row;
      gap: 15px;
    }
  }
  .nav-bot{
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: center;
    gap: 25px;
    align-items: center;


    div{
      display: flex;
      flex-direction: row;
      input{
        padding: 8px 25px;
        border: 0px;
        background-color: #f0f2f5;
      }
      .btn{
        padding: 5px 15px;
        background-color: #457993;
        color: white;
        border: 0px;
      }

    }
    a{
      text-decoration: none;
      color: black;
      span{
        color:#457993 ;
      }
    }

  }
}

</style>
