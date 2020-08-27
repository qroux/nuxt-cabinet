<template>
  <div class="container-fluid">
    <div class="banner-container">
      <div class="head-container fade-in one my-5">
        <h1>Docteur Gilbert Roux</h1>
        <hr />
        <h2>Chirurgien Dentiste</h2>
        <h2>9 rue Francis Davso, 13001 Marseille</h2>
      </div>
    </div>
    <div id="logos" class="container">
      <!-- <div class="presentation-container">
        <h5>Bienvenue au cabinet du docteur Gilbert Roux</h5>
        <br />
        <p>Le cabinet vous accueille</p>
      </div>-->
      <div class="logo-container py-5">
        <nuxt-link to="/implantologie" class="card-link px-5 py-4">
          <div class="logo text-center">
            <img src="~assets/test.png" alt />
            <hr />
            <h3>Implantologie</h3>
          </div>
        </nuxt-link>
        <nuxt-link to="/parodontologie" class="card-link px-5 py-4">
          <div class="logo text-center">
            <img src="~assets/logo-paro.png" alt />
            <hr />
            <h3>Parodontologie</h3>
          </div>
        </nuxt-link>
        <nuxt-link to="/soins" class="card-link px-5 py-4">
          <div class="logo text-center">
            <img src="~assets/question-logo.png" alt />
            <hr />
            <h3>Vos questions</h3>
          </div>
        </nuxt-link>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
.container-fluid {
  padding: 0;
}
.banner-container {
  min-height: 60vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-image: linear-gradient(rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.3)),
    url('~assets/banner3-resized.jpg');
  background-size: cover;
  @media (max-width: 740px) {
    background-image: linear-gradient(rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.3)),
      url('~assets/b2r.jpg') !important;
    // background-size: cover;
    background-position: center;
    h1 {
      font-size: 25px;
    }
    h2 {
      font-size: 20px;
    }
  }
}
#logos {
  font-family: 'Montserrat', sans-serif;
}

.presentation-container {
}

.logo-container {
  display: flex;
  justify-content: space-around;
  align-items: center;
  img {
    height: 110px;
    width: auto;
  }
  @media (max-width: 740px) {
    flex-direction: column;
    align-items: center;
    h3 {
      font-size: 22px;
    }
  }
}
.card-link {
  width: 300px;
  margin: 0;
  text-decoration: none;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
  transition: all 1s cubic-bezier(0.25, 0.8, 0.25, 1);
  color: rgba(0, 0, 0, 0.8);
  &:hover {
    box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25), 0 10px 10px rgba(0, 0, 0, 0.22);
  }
  @media (max-width: 740px) {
    margin-top: 20px;
  }
}
.head-container {
  text-align: center;
  color: white;
  padding: 2vh;
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
