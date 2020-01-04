<template>
  <div class="container-fluid full-container">
    <div class="head-container fade-in one">
      <h1>Docteur Gilbert Roux</h1>
      <hr />
      <h2>Chirurgien Dentiste</h2>
      <h2>Spécialisé en Implantologie et Parodontologie</h2>
    </div>
    <div class="actions-container">
      <div id="btn-size" class="btn btn-lg btn-info mx-2">Soins</div>
      <div id="btn-size" class="btn btn-lg btn-info mx-2">Info</div>
    </div>
  </div>
</template>

<script></script>

<style scoped lang="scss">
.full-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-image: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3)),
    url('https://picsum.photos/1920/1080.jpg');
  background-size: cover;
  height: 80vh;
  margin-bottom: 8.7vh;
}
.head-container {
  text-align: center;
  color: white;
  padding: 8vh;
}
.actions-container {
  margin-top: 20px;
  #btn-size {
    width: 150px;
    padding: 8px 0;
  }
}
@-webkit-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-moz-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

.fade-in {
  opacity: 0;
  -webkit-animation: fadeIn ease-in 1;
  -moz-animation: fadeIn ease-in 1;
  animation: fadeIn ease-in 1;

  -webkit-animation-fill-mode: forwards;
  -moz-animation-fill-mode: forwards;
  animation-fill-mode: forwards;

  -webkit-animation-duration: 1s;
  -moz-animation-duration: 1s;
  animation-duration: 1s;
  .one {
    -webkit-animation-delay: 1.5s;
    -moz-animation-delay: 1.5s;
    animation-delay: 1.5s;
  }
}
</style>
