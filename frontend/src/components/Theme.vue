<template>
<div>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
  <a class="navbar-brand" href="http://localhost:8080/">TOP10</a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto">
      <li class="nav-item active">
        <a class="nav-link" href="#">Музыка <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item active">
        <a class="nav-link" href="#">Кино <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item active">
        <a class="nav-link" href="#">Животные <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item active">
        <a class="nav-link" href="#">Наука <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item active">
        <a class="nav-link" href="#">Архитектура <span class="sr-only">(current)</span></a>
      </li><li class="nav-item active">
        <a class="nav-link" href="#">Техника <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item active">
        <a class="nav-link" href="#">Люди <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item active">
        <a class="nav-link" href="http://localhost:8080/create">Добавить <span class="sr-only">(current)</span></a>
      </li>
    </ul>
     <a class="nav-link" href="#">Вход</a>
    <form class="form-inline my-2 my-lg-0">
      <input class="form-control mr-sm-2" type="search" placeholder="Поиск" aria-label="Search">
      <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Найти</button>
    </form>
  </div>
</nav>
<div class="container">

</div>
  <footer class="footer text-center">
   <div class="containir"> 
      <img class="pic" src="../assets/vk.png">
      <img class="pic" src="../assets/facebook.png">
      <img class="pic" src="../assets/Telegram.png">
   </div>
  </footer>
</div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.footer {
  bottom: 0;
  width: 100%;
  height: 60px;
  line-height: 60px;
  background-color: #4b4747;
}
.topmy {
  background: #5aa2e0;
  font-size: 30px;
  text-align: center;
  color: #ffffff;
}
.pic {
  height: 30px;
}
</style>
