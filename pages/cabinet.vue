<template>
  <div class="full-container">
    <div class="container-fluid">
      <div class="article-bg">
        <h2>Cabinet</h2>
      </div>
    </div>
    <b-breadcrumb :items="items"></b-breadcrumb>
    <div class="container">
      <div class="full-article">
        <div class="article-content">
          <div class="header pt-3 pb-3">
            <h1 class="title">Présentation du cabinet</h1>
            <hr />
          </div>

          <b-container class="my-4">
            <!-- <b-row>
              <b-col cols="12">
                <p>Spécialisé en Implantologie et parodontologie, le docteur Gilbert Roux vous accueille dans son cabinet situé au 9 rue Francis Davso 13001 Marseille.</p>
                <p>Le cabinet est équipé de postes spécifiques à chaque type d'intervention, notamment pour la réalisation de chirurgies complexes.</p>
              </b-col>
            </b-row>-->
            <b-row>
              <b-col cols="12">
                <b-carousel
                  id="carousel-fade"
                  style="text-shadow: 0px 0px 2px #000"
                  fade
                  indicators
                  img-width="1024"
                  img-height="480"
                >
                  <b-carousel-slide
                    caption="Poste Chirurgie"
                    img-src="~assets/fauteuil2-1.jpg"
                    content-visible-up="xl"
                    class="modified"
                  ></b-carousel-slide>
                  <b-carousel-slide
                    caption="Poste Chirurgie"
                    img-src="~assets/b2r.jpg"
                    content-visible-up="xl"
                  ></b-carousel-slide>
                  <b-carousel-slide
                    caption="Poste Chirurgie"
                    img-src="~assets/fauteuil2-3.jpg"
                    content-visible-up="xl"
                  ></b-carousel-slide>
                  <b-carousel-slide
                    caption="Poste Parodontologie"
                    img-src="~assets/paro.jpg"
                    content-visible-up="xl"
                  ></b-carousel-slide>
                </b-carousel>
              </b-col>
            </b-row>
          </b-container>
          <br />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import FsLightbox from 'fslightbox-vue'
export default {
  components: { FsLightbox },
  data() {
    return {
      toggler: false,
      items: [
        {
          text: 'Accueil',
          to: { name: 'index' }
        },
        {
          text: 'Cabinet',
          active: true
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
$animate: all 0.2s ease-in-out;

.full-container {
  min-height: 72vh;
}
.container-fluid {
  padding: 0;
}
.article-bg {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 10vh;
  color: white;
  text-align: center;
  background-image: url('~assets/paro.jpg');
  background-position: center;
  background-size: cover;
}
.full-article {
  display: flex;
  flex-direction: column;
}

@media screen and (max-width: 768px) {
  h1 {
    font-size: 30px;
  }
  h3 {
    font-size: 25px;
  }
}

hr {
  padding: 0;
  margin: 0;
}

.title {
  color: rgba(0, 0, 0, 0.7);
  font-weight: bold;
}

.breadcrumb {
  background-color: #f2f2f2;
}
</style>
