<script></script>
<template>
  <header class="header">
    <div class="container">
      <div class="adres">
        <p class="adres__text  animate__animated animate__slideInLeft">Новокузнечный переулок 4/1</p>
        <p class="adres__text  animate__animated animate__slideInRight">8 (812) 123-45-67</p>
      </div>
      <nav class="header__nav  animate__animated animate__slideInLeft">
        <ul class="nav-list">
          <li class="list-item" style="border-left: none; border-right: none;"><a href="#" class="nav__link">Каталог</a></li>
          <li class="list-item" style="border-right: none;"><a href="#" class="nav__link">Доставка</a></li>
          <li class="list-item" style="border-right: none;"><a href="#" class="nav__link">Коллекции</a></li>
          <li class="list-item" style="border-right: none;"><a href="#" class="nav__link">Контакты</a></li>
        </ul>
      </nav>
    </div>
  </header>  
</template>
<style lang="scss" scoped>
.header {
  width: 100%;
  .container {
    display: flex;
    flex-direction: column;
  }  
}

.adres {
  width: 100%;
  height: 70px;
  display: flex;
  justify-content: space-between;  
  align-items: center;
}

.adres__text {
  color: #FFF;
  font-family: Montserrat;
  font-size: 13px;    
  font-weight: 500;
}

.header__nav {
  min-width: 100%;  
  border-bottom: 1px solid #fff;
  border-top: 1px solid #fff;
}
.nav-list {
  max-width: 100%;
  display: flex;
  flex-direction: row;  
  justify-content: space-between;
}
.list-item {
  list-style-type: none;  
  padding: 10px 100px;
  border-left: 1px solid #fff;
  border-right: 1px solid #fff;
}
.nav__link {
  font-family: Montserrat;
  font-size: 14px;
  font-weight: 400;  
  color: #FFF;
  text-decoration: none;
  transition: .3s;
  &:hover {
    color: #99862A;
    transition: all .3s;
  }
}

@media (max-width: 1199px) {
  .list-item {
    padding: 10px 53px;
  }  
}
@media (max-width: 767px) {
  .list-item {
    padding: 10px 30px;
  }  
}
@media (max-width: 575px) {
  .header__nav {
    border: none;
  }  
  .nav-list {
    flex-direction: column;
}  
.list-item {
    width: 100%;
    border: none;
    &:nth-of-type(even) {
      border-bottom: 1px solid #fff;  
      border-top: 1px solid #fff;  
    }
    &:last-child {
      border-top: 1px solid #fff;
    }
    display: flex;
    justify-content: center;
    
  }  

  .adres__text {
    font-size: 11px;
  }
}
</style>