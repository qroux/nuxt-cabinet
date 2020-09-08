<template>
  <div class="container full-container">
    <b-tabs
      active-nav-item-class="my-active"
      active-tab-class
      class="mt-5 full-tab custom-tabs"
      content-class="mt-5"
      fill
    >
      <b-tab>
        <template v-slot:title>
          <h3>Catégories</h3>
        </template>
        <b-card-group deck class="pb-5">
          <b-card
            v-for="card in cards"
            v-bind:key="card.title"
            tag="nuxt-link"
            :to="card.link"
            :img-src="card.src"
            img-alt="Card image"
            img-top
            :header="card.title"
          >
            <ul>
              <li>Méthode Charon</li>
            </ul>
          </b-card>
        </b-card-group>
      </b-tab>
      <b-tab>
        <template v-slot:title>
          <h3>Questions</h3>
        </template>
        <div v-for="question in questions" v-bind:key="question.title" class="py-2">
          <nuxt-link :to="question.link" class="questions">
            <h5>{{ question.title }}</h5>
          </nuxt-link>
        </div>
      </b-tab>
    </b-tabs>
  </div>
</template>

<script>
export default {
  props: {
    cards: {
      default: () => [
        {
          title: 'Parodontologie',
          link: '/parodontologie',
          src: '/images/soins/ss-paro.webp',
          subtitles: ['Méthode Charon']
        },
        {
          title: 'Endodontie',
          link: '/endodontie',
          src: '/images/soins/ss-endo.webp',
          subtitles: ['Traitement des racines']
        },
        {
          title: 'Esthétique',
          link: '/implantologie',
          src: '/images/soins/ss-facettes2.jpg',
          subtitles: ['Implants']
        }
      ]
    },
    questions: {
      default: () => [
        {
          title:
            "J'ai peur d'aller chez le dentiste, comment me faire soigner ?",
          link: '/questions/dentophobie'
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
.full-container {
  display: flex;
  justify-content: center;
  min-height: 72vh;
}
.card {
  text-decoration: none;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
  transition: all 1s cubic-bezier(0.25, 0.8, 0.25, 1);
  color: rgba(0, 0, 0, 0.8);
  &:hover {
    box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25), 0 10px 10px rgba(0, 0, 0, 0.22);
  }
  .card-title {
    text-align: center;
  }
}
h2 {
  &:hover {
    font-weight: bold;
    cursor: pointer;
  }
}
.full-tab {
  width: 100%;
}

.custom-tabs {
  font-size: 25px !important;
}
h3 {
  color: rgba(0, 0, 0, 0.4);
}
.my-active {
  h3 {
    font-weight: bold !important;
    color: rgba(0, 0, 0, 0.7);
  }
}

.questions {
  color: rgba(0, 0, 0, 0.5);
  transition: 0.5s;
  text-decoration: none;
  &:hover {
    color: rgba(0, 0, 0, 1);
  }
  h5:hover {
    font-weight: bold;
  }
}

h6 {
  padding-top: 10px;
}

ul {
  list-style-type: none;
  font-size: 15px;
  padding: 0px 15px;

  li:before {
    content: '\00b7	\00a0	\00a0	';
  }
}

img {
  max-height: 200px;
}

// .card {
//   min-height: 400px;
// }

.card-title {
  font-weight: bold;
}

.card-header {
  // background-color: #262b36;
  text-align: center;
  font-weight: bold;
}
</style>
