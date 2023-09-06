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
    <section class="novinki">
      <div class="container">
        <div class="left">
          <p class="upper-text">Новинки коллекций</p>
          <h1 class="title">Март 1980 Урожай Марселя</h1>
          <div class="line"></div>
          <p class="text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Feugiat enim tortor in hac id imperdiet adipiscing. Pellentesque nisi, mi sit non sit sed fermentum. Felis adipiscing morbi sodales ac. </p>
          <table class="table-for-date">
            <tr>
              <td class="date">1980</td>
              <td class="table-text">Colli Euganei Bianco Ca' Lustra 1980 <span>Красочная бутылка вина из Марселя</span></td>
            </tr>
            <tr>
              <td class="date" style="border-bottom:1px solid #282828; border-top:1px solid #282828;">1980</td>
              <td class="table-text" style="border-bottom:1px solid #282828; border-top:1px solid #282828;">Colli Euganei Bianco Ca' Lustra 1980 <span>Красочная бутылка вина из Марселя</span></td>
            </tr>
            <tr>
              <td class="date">1980</td>
              <td class="table-text">Colli Euganei Bianco Ca' Lustra 1980 <span>Красочная бутылка вина из Марселя</span></td>
            </tr>
          </table>
          <p class="text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Feugiat enim tortor in hac id imperdiet adipiscing. Pellentesque nisi, mi sit non sit sed fermentum. Felis adipiscing morbi sodales ac. </p>
          <a href="#" class="btn">узнать подробнее</a>
        </div>
        <img src="./assets/img/img/novinki/Group 4.png" alt="" class="right">
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

.novinki {
  background: #E6E3C4;
  padding: 80px 0px 80px 0px;
  .container {
    padding: 60px 0px 60px 0px;
    display: flex;
    justify-content: space-between;
  }
}
.left {
  height: 758px;
  width: 445px;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
}
.upper-text {
  font-family: Montserrat;
  font-size: 16px;
  font-weight: 400;
  margin-bottom: 30px;
}
.title {
  color: var(--black, #282828);
  font-family: Playfair_Display;
  font-size: 36px;
  font-weight: 700;
  margin-bottom: 30px;
}
.line {
  width: 160px;
  height: 1px;
  background: var(--black, #282828);
  margin-bottom: 30px;
}
.text {
  color: var(--black, #282828);
  font-family: Montserrat;
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  margin-bottom: 30px;
}
.table-for-date {
  height: 228px;
  width: 100%;
  margin-bottom: 30px;
}
.date {
  padding: 24px;
  color: var(--black, #282828);
  font-family: Montserrat;
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  border-right: 1px solid #282828;
}
.table-text {
  padding: 15px 30px;
  color: var(--black, #282828);
  font-family: Playfair Display;
  font-size: 18px;
  font-style: normal;
  font-weight: 700;
  line-height: 150%;
  span {
    color: var(--black, #282828);
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
  }
}
.btn {
  color: var(--white, #FFF);
  font-family: Montserrat;
  font-size: 16px;
  font-weight: 500;
  width: 250px;
  height: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  background: var(--accent, #998431);
  border: 2px solid #998431;
  transition: .3s;
  text-decoration: none;
  &:hover {
    background: none;
    color: #998431;
    transition: all .3s;
  }
}
@media (max-width: 1199px) {
  .novinki {
    .container {
      flex-direction: column-reverse;
    }
  }
}
@media (max-width: 575px) {
  .table-for-date {
    display: none;
  }
  .left {
    height: 400px;
    width: 290px;
  }
}
</style>
