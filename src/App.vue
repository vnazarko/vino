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
        <img src="./assets/img/img/novinki/Group.png" alt="" class="right">
      </div>
    </section>
    <section class="record">
      <div class="container">
        <div class="top">
          <img src="./assets/img/img/record/grape.png" alt="" class="record__img">
          <div class="center">
            <h1 class="record__title">Запись на дегустацию</h1>
            <div class="line"></div>
            <p class="record__text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Feugiat enim tortor in hac id imperdiet adipiscing. Pellentesque nisi, mi sit non sit sed fermentum. </p>
          </div>
          <img src="./assets/img/img/record/image.png" style="width:260px; height:200px;" alt="" class="record__img">
        </div>
        <div class="bottom">
          <form class="form">
            <div class="inline">
              <ul class="inline__list">
                <li class="inline__item">
                  <input type="text" placeholder="Имя" class="input">
                </li>
                <li class="inline__item">
                  <input type="number" placeholder="Телефон" class="input">
                </li>
              </ul>
            </div>
            <p class="place">Бутик на Невском 103</p>
            <a href="#" class="form__btn">записаться</a>
          </form>
        </div>
      </div>
    </section>
    <footer class="footer">
      <div class="container">
        <nav class="footer__nav">
          <ul class="footer__nav-list">
            <li class="list-item"><a href="#" class="nav__link">Главная</a></li>
            <li class="list-item"><a href="#" class="nav__link">Каталог</a></li>
            <li class="list-item"><a href="#" class="nav__link">Поставщики</a></li>
            <li class="list-item"><a href="#" class="nav__link">Коллекции</a></li>
            <li class="list-item"><a href="#" class="nav__link">Дегустация</a></li>
            <li class="list-item"><a href="#" class="nav__link">Коллекции 2020</a></li>
            <li class="list-item"><a href="#" class="nav__link">Контакты</a></li>
          </ul>
        </nav>
        <nav class="connect">
          <ul class="connect__list">
            <li class="list-item">винный бутик le corte</li>
            <li class="list-item">8 (812) 123-45-67</li>
            <li class="list-item">© le-corte.ru</li>
          </ul>
        </nav>
      </div>
    </footer>
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
  text-transform: uppercase;
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
  .novinki {
    height: 1200px;
  }
  .table-for-date {
    display: none;
  }
  .left {
    height: 400px;
    width: 290px;
  }
}

// record

.record {
  width: 100%;
  padding: 100px 0px;
  .container {
    display: flex;
    flex-direction: column;
    padding-bottom: 80px;
  }
}
.top {
  max-width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.record__img {
}
.line {
  width: 118px;
  height: 1px;
  border: none;
  background: #FFF;
  margin: 40px auto 40px auto;
}
.record__title {
  color: var(--white, #FFF);
  text-align: center;
  font-family: Playfair Display;
  font-size: 36px;
  font-weight: 700;
}
.record__text {
  max-width: 539px;
  color: var(--white, #FFF);
  text-align: center;
  font-family: Montserrat;
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  margin-left: auto;
  margin-right: auto; 
}

.bottom {
  height: 340px;
  border: 3px solid #C4C4C4;
  border-top: none;
}
.form {
  max-width: 540px;
  display: flex;
  flex-direction: column;
  margin: 80px auto 0 auto;
}
.inline {
  max-width: 100%;
  display: flex;
  justify-content: space-between;
}

.inline__list {
  display: flex;
  flex-direction: row;
  width: 100%;
  justify-content: space-between;  
}

.inline__item {
  list-style-type: none;
  padding-bottom: 5px;
  border-bottom: 1px solid var(--white, #FFF);
}

.input {
  width: 254px;
  border-bottom: 1px solid #fff;
  color: var(--white, #FFF);
  font-family: Montserrat;
  font-size: 13px;
  font-style: normal;
  font-weight: 500;
  background: none;
  border: none;
  &::placeholder {
    color: var(--white, #FFF);
    font-family: Montserrat;
    font-size: 13px;
    font-style: normal;
    font-weight: 500;
    padding-bottom: 20px;
    border: none;
    border-bottom: 1px solid #fff;
  }
}
.place {
  color: var(--white, #FFF);
  font-family: Montserrat;
  font-size: 13px;
  font-style: normal;
  font-weight: 500;
  max-width: 100%;
  padding-bottom: 10px;
  border-bottom: 1px solid #fff;
  margin-top: 40px;
}
.form__btn {
  color: var(--white, #FFF);
  font-family: Montserrat;
  font-size: 16px;
  font-style: normal;
  font-weight: 500;
  width: 100%;
  height: 50px;
  text-transform: uppercase;
  border: 1px solid var(--white, #FFF);
  margin-top: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  text-decoration: none;
  transition: .3s;
  &:hover {
    background: #fff;
    color: #282828;
    transition: all .3s;
  }
}

@media (max-width: 1199px) {
  .record__img {
    display: none;
  }
  .center {
    margin: 0 auto;
  }
}
@media (max-width: 767px) {
  .inline__list {
    flex-direction: column;
  }
  .bottom {
    border: none;
  }
}

@media (max-width: 575px) {
  .record {
    height: 750px;
  }
}

// footer 

.footer {
  padding: 50px 0px 50px;
  background: var(--accent, #998431);
  width: 100%;
}
.footer__nav {
  width: 100%;
}
.footer__nav-list {
  width: 100%;
  display: flex;
  justify-content: space-evenly;
  flex-direction: row;
  border-bottom: 1px solid #fff;
  border-top: 1px solid #fff;
  flex-wrap: wrap;
  .list-item {
    padding-top: 20px;
    padding-bottom: 20px;
    list-style-type: none;
    padding-left: 20px;
  }
  .nav__link {
    color: var(--white, #FFF);
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    text-decoration: none;
    transition: .3s;
    &:hover {
      color: #282828;
      transition: all .3s;
    }
  }
}
.connect {
  width: 100%;
  border-bottom: 1px solid #fff;
}
.connect__list {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  flex-wrap: wrap;
  .list-item {
    color: var(--white, #FFF);
    text-align: center;
    font-family: Montserrat;
    font-size: 14px;
    font-style: normal;
    font-weight: 600;
    line-height: 150%; /* 21px */
    text-transform: uppercase;
    list-style-type: none;
    padding-top: 20px;
    padding-bottom: 20px;
    padding-left: 20px;
  }
}
</style>
