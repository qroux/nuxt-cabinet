<template>
  <div class="full-container">
    <div class="container-fluid">
      <div class="article-bg">
        <h2>Parodontologie</h2>
      </div>
    </div>
    <b-breadcrumb :items="items"></b-breadcrumb>
    <div class="container">
      <div class="full-article">
        <div class="article-content">
          <div class="header pt-3 pb-3">
            <h1 class="title">Douleurs, déchaussement, comment traiter une parondontite ?</h1>
            <hr />
          </div>

          <b-container class="my-4">
            <b-row>
              <b-col cols="12">
                <p>
                  Le "déchaussement" des dents porte le nom médical de "maladies
                  parodontales".
                  <strong>
                    Ce sont une série de maladies qui se caractérisent par la
                    destruction, plus ou moins sévère, plus ou moins rapide, du
                    parodonte, c'est-à-dire des tissus qui soutiennent vos
                    dents.
                  </strong>
                </p>
              </b-col>
            </b-row>
          </b-container>
          <br />

          <b-container>
            <SubChapter
              v-for="(chapter, index) of chaptersContent"
              :key="chapter.title"
              :title="chapter.title"
              :num="index"
            >
              <template v-slot:content>
                <span v-html="chapter.content"></span>
              </template>
            </SubChapter>
          </b-container>

          <br />
          <br />

          <div id="ligthbox" class="mt-3 mb-5">
            <h3 class="font-weight-bold">Cas cliniques</h3>
            <hr class="mb-4" />

            <div class>
              <div @click="toggler = !toggler">
                <b-container fluid class="thumbnails-container justify-content-between">
                  <b-row>
                    <b-col cols="12" md="3">
                      <b-img thumbnail fluid src="/images/paro/paro-min1.png" alt="Image 1"></b-img>
                    </b-col>
                    <b-col cols="12" md="3">
                      <b-img thumbnail fluid src="/images/paro/paro-min2.png" alt="Image 1"></b-img>
                    </b-col>
                  </b-row>
                </b-container>
              </div>
            </div>

            <FsLightbox
              :toggler="toggler"
              :sources="[
                '/images/paro/paro-min1.png',
                '/images/paro/paro-min2.png',
                '/images/paro/paro1.png',
                '/images/paro/paro2.png',
                '/images/paro/paro3.png'
              ]"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import SubChapter from '../components/articles/SubChapter'
import FsLightbox from 'fslightbox-vue'
import { BIconChevronDown, BIconChevronCompactDown } from 'bootstrap-vue'

export default {
  components: {
    SubChapter,
    FsLightbox,
    BIconChevronDown,
    BIconChevronCompactDown
  },
  data() {
    return {
      toggler: false,
      chaptersContent: [
        {
          title: 'Pourquoi la parodontite se manifeste-t-elle maintenant ?',
          content: `            <p>
              Pour déclencher une parondite, il faut deux conditions : L'une
              sans l'autre ne peut pas détruire les tissus parodontaux.
              <br />
              <br />
              <strong>
                Dans la plupart des cas, il s'agit d'une infection chronique qui
                évolue par la succession d'épisodes d'activité
              </strong>
              (souvent sans que vous vous en rendiez compte) entrecoupés de
              périodes de repos.
              <br />
              <strong>
                Le terrain immunitaire et la flore bactérienne de chacun.
              </strong>{' '}
              Ces parodontites apparaissent chez certains individus et pas chez
              d'autres : nous ne sommes pas tous susceptibles de souffrir de
              parondontite / d'un déchaussement.
            </p>`
        },
        {
          title:
            "Quelles sont les risques de d'apparition et de récidives d'une parodontite ?",
          content: `<p>Les principaux facteurs de risque sont :</p>

            <ul>
              <li>
                Présence
                <strong>
                  d'antécédents
                  familiaux
                </strong> de parodontite.
              </li>
              <li>
                Présence de
                <strong>stress</strong> accompagné d'anxiété.
              </li>
              <li>
                Consommation excessive de
                <strong>tabac</strong>.
              </li>
              <li>
                État médical où le sujet est
                sensible aux infections
                <strong>(diabète par exemple)</strong>.
              </li>
              <li>
                <strong>
                  Résistance à la
                  carie dentaire
                </strong>.
              </li>
              <li>
                Historique d'infection gingivale sévère
                (gingivite).
              </li>
            </ul>`
        },
        {
          title: 'Comment prévenir une parodontite / un déchaussement ?',
          content: `            <p>
              Il existe aujourd’hui des
              <strong>
                moyens modernes de prévenir efficacement
                le déchaussement
              </strong> dont notre cabinet peut vous informer utilement.
              De plus le Dr Roux, Parodontiste est à même,
              <strong>
                après un entretien et
                des examens précis, de déterminer la nature exacte du risque de
                votre déchaussement
              </strong> car il existe des sujets plus à risque que
              d’autres de souffrir de déchaussement ou parodontite.
            </p>
            <p>
              En terme de prévention, après évaluation de votre degré de risque
              de voir vos dents se déchausser,
              <strong>
                un programme simple, peu coûteux
                et adapté à votre risque, permet de diminuer sensiblement la
                probabilité de déchaussement
              </strong>
            </p>`
        },
        {
          title: 'Conclusion',
          content: `<p>
              Prévenir, c'est
              <strong>
                évaluer l'intensité du risque et diminuer ce
                risque grâce à un traitement préventif.
              </strong>
            </p>
            <p>
              Au total,
              <strong>il est bien plus agréable et moins coûteux de garder ses dents</strong> que
              de les perdre à condition d’avoir les bons réflexes et de
              bénéficier d’outils thérapeutiques opérants.
            </p>`
        }
      ],
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
          text: 'Parodontologie',
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
.icon-margin {
  margin-left: 2vw;
}

@media screen and (max-width: 768px) {
  h1 {
    font-size: 30px;
  }
  h3 {
    font-size: 25px;
  }

  // .dotted {
  //   margin-bottom: 25px;
  // }
  .icon-margin {
    margin-left: 5vw;
  }
}

hr {
  padding: 0;
  margin: 0;
}

// .dotted {
//   &:before {
//     content: '\00b7	\00a0	\00a0';
//   }

//   color: rgba(0, 0, 0, 0.7);
//   &:hover {
//     cursor: pointer;
//     color: rgba(0, 0, 0, 1);
//   }
// }
.title {
  color: rgba(0, 0, 0, 0.7);
  font-weight: bold;
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
