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
</style>
