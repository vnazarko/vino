<script>
import Header from "./components/Header.vue"

export default {
  components: {
    Header,
  }
}
</script>

<template>
  <div class="wrapper">
    <div class="intro">
      <Header/>
      <div class="container">
        <div class="intro__buttons">
          <a href="#" class="intro__btn">винная карта</a>
          <a href="#" class="intro__btn">дегустация</a>
        </div>
      </div>
    </div>
    <section class="quote">
      <div class="container">
        <h1 class="title">Лучший вкус, это вкус долголетнего вина</h1>
        <div class="line"></div>
        <p class="text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Feugiat enim tortor in hac id imperdiet adipiscing. Pellentesque nisi, mi sit non sit sed fermentum. Felis adipiscing morbi sodales ac. Mauris dictumst risus pulvinar blandit elit. Vestibulum quam ultrices nascetur et viverra suscipit. Proin vitae aliquet leo aliquam amet rutrum. Lectus auctor purus ultrices enim ultrices. Augue fringilla tellus tortor orci ultrices sed. Viverra cras sapien, pellentesque viverra malesuada. Tellus dolor, eget vitae dignissim molestie eget sit duis. Vitae dui vel pretium euismod diam. Pellentesque amet, lacus, amet, quis risus. Pellentesque scelerisque nunc, orci aliquam quis.</p>
        <img src="./assets/img/img/quote/image.png" alt="" class="img">
      </div>
    </section>
  </div>
</template>

<style scoped lang="scss">
// intro 

.intro {
  height: 900px;
  background-image: url('./assets/img/img/bgc.png');
}

.intro__buttons {
  width: 415px;
  height: 50px;
  margin: 583px auto 0px auto;
  display: flex;
  justify-content: space-between;
}

.intro__btn {
  color: #FFF;
  font-family: Montserrat;
  font-size: 16px;
  font-weight: 500;
  text-transform: uppercase;  
  padding: 15px 30px;
  text-decoration: none;
  background: #99862A;
  border: 2px solid #99862A;
  transition: .3s;
  &:hover {
    border: 2px solid #99862A;
    background: none;
    transition: all .3s;
  }
}

@media (max-width: 575px) {
  .intro__buttons {
    width: 100%;
    display: flex;
    flex-direction: column;
    margin-top: 400px;
  }

  .intro__btn {
    display: flex;
    justify-content: center;
    margin-top: 15px;
  }
}

// quote

.quote {
  width: 100%;
  .container {
    padding-bottom: 60px;
    padding-top: 60px;
    border: 3px solid #C4C4C4;
    margin-top: 100px;
    margin-bottom: 100px;
    display: flex;
    justify-content: center;
    flex-direction: column;
    padding: 20px;
  }  

  .title {
    color: #FFF;
    font-family: Playfair Display;
    font-size: 36px;
    font-style: normal;
    font-weight: 700;
    text-align: center;
  }

  .line {
    width:160px; 
    height: 1px;
    border:none; 
    background:#fff; 
    margin: 40px auto;
  }

  .text {
    max-width: 733px;
    color: #FFF;
    text-align: center;
    font-family: Montserrat;
    font-size: 16px;
    font-weight: 400;
    margin: 0 auto 50px auto;
  }

  .img {
    width: 160px;
    height: 160px;
    margin: 0 auto;
  }
}
</style>
