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
        <a class="nav-link" href="#">Другое <span class="sr-only">(current)</span></a>
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
        <div class="form-group">
            <label for="exampleFormControlInput1">Выберите название темы</label>
            <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="Тема">
        </div>
        <div class="form-group">
            <label for="exampleFormControlTextarea1">Описание темы</label>
            <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
        </div>
        <select class="form-control">
            <option selected>Выберите раздел для вашей темы</option>
            <option value="1">Музыка</option>
            <option value="2">Кино</option>
            <option value="3">Животные</option>
        </select>
       <div class="custom-file" style="margin: 15px 0px;">
            <input type="file" class="custom-file-input" id="customFile">
            <label class="custom-file-label" for="customFile">Выберите картинку для вашей темы</label>
        </div>
        <div v-for="numb in numbers">
            <div class="form-group">
            <label for="exampleFormControlInput1">Объект №{{numb}}</label>
            <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="Название">
        </div>
        <div class="form-group">
            <textarea class="form-control" id="exampleFormControlTextarea1" placeholder="Описание" rows="3"></textarea>
        </div>
       <div class="custom-file" style="margin: 15px 0px;">
            <input type="file" class="custom-file-input" id="customFile">
            <label class="custom-file-label" for="customFile">Выберите картинку для объекта</label>
        </div>
        </div> 
        <button type="button" class="btn btn-primary" style="margin: 0px 0px 15px 0px;">Добавить</button>
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
  name: "Create",
  data() {
    return {
      numbers: [1,10],
    };
  },
  mounted() {
    this.loadNumbers();
  },
  methods: {
    loadNumbers() {
      var numbers = [];
      for(var i=1; i<11; i++){
          numbers[i-1]=i;
      }
      this.numbers=numbers;
    },
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
