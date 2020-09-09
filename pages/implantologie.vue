<template>
  <div class="full-container">
    <div class="container-fluid">
      <div class="article-bg">
        <h2>Implantologie</h2>
      </div>
    </div>
    <b-breadcrumb :items="items"></b-breadcrumb>
    <div class="container">
      <div class="full-article">
        <div class="article-content">
          <div class="header pt-3 pb-3">
            <h1 class="title">Les implants dentaires, quand y recourir ?</h1>
            <hr />
          </div>

          <b-container class="my-4">
            <b-row>
              <b-col cols="12">
                <p>En construction</p>
              </b-col>
            </b-row>
          </b-container>
          <br />

          <div id="ligthbox" class="mt-3 mb-5">
            <h3 class="font-weight-bold">Cas cliniques</h3>
            <hr class="mb-4" />

            <div class>
              <div @click="toggler = !toggler">
                <b-container fluid class="thumbnails-container justify-content-between">
                  <b-row>
                    <b-col cols="12" md="3">
                      <b-img thumbnail fluid src="/images/implanto/implanto0.jpg" alt="Image 1"></b-img>
                    </b-col>
                    <b-col cols="12" md="3">
                      <b-img thumbnail fluid src="/images/implanto/implanto5.jpg" alt="Image 1"></b-img>
                    </b-col>
                  </b-row>
                </b-container>
              </div>
            </div>

            <FsLightbox
              :toggler="toggler"
              :sources="[
                '/images/implanto/implanto0.jpg',
                '/images/implanto/implanto2.jpg',
                '/images/implanto/implanto3.jpg',
                '/images/implanto/implanto4.jpg',
                '/images/implanto/implanto5.jpg',
                '/images/implanto/implanto6.jpg'
              ]"
            />
          </div>
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
          text: 'Soins',
          to: { name: 'soins' }
        },
        {
          text: 'Implantologie',
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
    // &:before {
    //   content: '\25b6	\00a0	\00a0	\00a0 \00a0';
    // }
  }

  .dotted {
    margin-bottom: 25px;
  }
}

hr {
  padding: 0;
  margin: 0;
}

.dotted {
  &:before {
    content: '\00b7	\00a0	\00a0';
  }

  color: rgba(0, 0, 0, 0.7);
  &:hover {
    cursor: pointer;
    color: rgba(0, 0, 0, 1);
  }
}
.title {
  color: rgba(0, 0, 0, 0.7);
  font-weight: bold;
}

.photo {
  // height: 50%;
  background-image: url('~assets/ss-endo3.webp');
}

.thumbnails-container {
  &:hover {
    cursor: pointer;
  }
}

.breadcrumb {
  background-color: #f2f2f2;
}
</style>
