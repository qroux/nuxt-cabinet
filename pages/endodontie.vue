<template>
  <div class="full-container">
    <div class="container-fluid">
      <div class="article-bg">
        <h2>Endodontie</h2>
      </div>
    </div>
    <b-breadcrumb :items="items"></b-breadcrumb>
    <div class="container">
      <div class="full-article">
        <div class="article-content">
          <div class="header pt-3 pb-3">
            <h1 class="title">Le traitement des racines, pourquoi et comment ?</h1>
            <hr />
          </div>

          <b-container class="my-4">
            <b-row>
              <b-col cols="12">
                <p>
                  Dans de rares cas, il peut arriver qu’un traitement de racine
                  (=endodontique) ne fonctionne pas comme prévu. La dent traitée
                  pourrait ne pas guérir correctement ou le patient pourrait
                  éprouver des complications post-opératoires qui compromettent
                  la dent.
                </p>
                <p>
                  La reprise d’un traitement endodontique consiste à enlever la
                  couronne et les matériaux d'obturation précédents, à nettoyer
                  les canaux radiculaires, et à réapposer un matériau
                  d'obturation et une couronne prothétique sur la dent. En bref,
                  la reprise d’un traitement endodontique est presque identique
                  à la procédure initiale, hormis le retrait des structures du
                  premier traitement.
                  <strong>
                    Le taux de réussite pour une reprise d’un traitement
                    endodontique se situe à 75 %.
                  </strong>
                  <br />
                  <br />
                  <strong>
                    Les traitements endodontiques et les reprises sont une
                    meilleure alternative que l'extraction dentaire pour la
                    plupart des patients.
                  </strong>
                  Si une dent a un bon soutien osseux, une surface solide et une
                  gencive saine, elle a de bonnes chances d'être préservée.
                  <br />Opter pour la reprise d’un traitement endodontique peut
                  être beaucoup moins coûteux que les solutions alternatives.
                  Les implants dentaires, les ponts multiples et la création de
                  dents prothétiques esthétiques coûtent beaucoup plus chers que
                  de travailler sur une dent naturelle. Ces solutions exigent
                  également un entretien et apportent une sensation moins
                  naturelle qu'une « vraie » dent.
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
                      <b-img
                        thumbnail
                        fluid
                        src="/images/endo/endo2-2.png"
                        alt="Image 1"
                        class="mx-auto d-block"
                      ></b-img>
                    </b-col>
                    <b-col cols="12" md="3">
                      <b-img
                        thumbnail
                        fluid
                        src="/images/endo/endo2-4.png"
                        alt="Image 1"
                        class="mx-auto d-block"
                      ></b-img>
                    </b-col>

                    <b-col cols="12" md="3">
                      <b-img
                        thumbnail
                        fluid
                        src="/images/endo/endo2-6.png"
                        alt="Image 1"
                        class="mx-auto d-block"
                      ></b-img>
                    </b-col>
                  </b-row>
                </b-container>
              </div>
            </div>

            <FsLightbox
              :toggler="toggler"
              :sources="[
                '/images/endo/endo1-2.png',
                '/images/endo/endo2-1.png',
                '/images/endo/endo2-2.png',
                '/images/endo/endo2-3.png',
                '/images/endo/endo2-4.png',
                '/images/endo/endo2-5.png',
                '/images/endo/endo2-6.png'
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

export default {
  components: { SubChapter, FsLightbox },
  data() {
    return {
      toggler: false,
      chaptersContent: [
        {
          title:
            'Pourquoi la reprise d’un traitement de racine est-elle nécessaire ?',
          content: `<p>
              Il y a un certain nombre de raisons pour lesquelles un traitement
              endodontique initial échoue de manière inattendue, incluant :
            </p>
            <ul>
              <li>Une couronne fracturée avec une fuite du matériau d’obturation</li>
              <li>
                Des canaux courbés ou étroits qui n’ont pas été traités au cours
                de la procédure initiale
              </li>
              <li>
                Un retard dans la mise en place des restaurations après la
                procédure initiale
              </li>
              <li>Une nouvelle carie sur la dent traitée</li>
              <li>Une nouvelle fracture sur la dent traitée</li>
              <li>Des structures endodontiques complexes à ramifications multiples</li>
            </ul>
            <p>
              <strong>
                Bien que la perspective d'une chirurgie endodontique
                additionnelle puisse sembler désagréable, la reprise d’un
                traitement endodontique est assez simple. En général, l'ensemble
                du traitement peut être complété en 1 à 3 visites.
              </strong>
            </p>`
        },
        {
          title: 'En quoi consiste la reprise d’un traitement endodontique ?',
          content: `<p>
              Le jour de la procédure de la reprise d’un traitement
              endodontique, une anesthésie locale sera réalisé. La longueur du
              rendez-vous dépend en partie de l'inflammation et de la complexité
              du traitement.
            </p>
            <p>
              La première étape d'une reprise de traitement endodontique est
              d'accéder à la portion intérieure de la dent. Si une couronne et
              un tenon ont été insérés, ils seront enlevés.
              <br />
              <br />Ensuite, le matériau d’obturation et les obstructions qui
              bloquent les canaux radiculaires seront enlevés. Ce retrait est
              effectué en utilisant une pièce à main ultrasonique. L'avantage
              d'utiliser cet outil est que tout matériau indésirable est relâché
              par vibrations. De minuscules instruments seront ensuite utilisés
              pour nettoyer et remodeler les canaux radiculaires. Des
              radiographies peuvent être prises pour s’assurer de la progression
              du débouchage et à la fin pour vérifier que les racines sont bien
              propres et libres pour une nouvelle obturation étanche. Si cette
              partie du traitement s'avère plus complexe, une pause sera faite.
              La fin de la procédure de nettoyage sera alors effectuée lors de
              la visite suivante.
              <br />
              <br />Lorsque le dentiste a validé que les canaux sont
              complètement nettoyés et libre d’accès il procède au rebouchage.
              Un ciment d’étanchéité et des cônes de gutta-percha sont utilisés
              pour obturer les racines et les sceller hermétiquement. Cette
              procédure permet la guérison de la dent en la protégeant des
              bactéries et donc des infections. Enfin, une obturation provisoire
              est placée dans la dent. Dans la séance suivante la dent reçoit
              une reconstitution interne pour renforcer sa partie centrale que
              la carie a détruite. Cette dent traitée au niveau des racines et
              maintenant renforcée en son centre doit être néanmoins recouverte
              par une couronne pour la protéger totalement et lui redonner son
              esthétique.
            </p>`
        },
        {
          title: 'Les limites du traintement des racines',
          content: `<p>
              En dépit des efforts, du temps, et des précautions opératoires
              certaines dents peuvent ne pas atteindre le degré de sécurité long
              terme recherché. Les Raisons sont liées à certains obstacles:
            </p>
            <ul>
              <li>
                La complexité radiculaire initiale. Courbure très marquées,
                ramification…
              </li>
              <li>
                Le retraitement peut trouver l’intérieur des racines des parties
                métalliques qui ne peuvent être retirées
              </li>
              <li>
                Le retraitement peut trouver l’intérieur des dents très
                fragilisé tenant compte de leur finesse ou leur déminéralisation
                par la carie.
              </li>
              <li>
                Le retraitement rencontre également un intérieur des canaux des
                fois, très modifiés dans leur courbure naturelle d’origine. On
                peut rencontrer des butées, ou des trajets rectilignes (appelés
                faux canaux) ressortant latéralement à la racine et non à son
                extrémité.
              </li>
              <li>Une nouvelle fracture sur la dent traitée</li>

              <li>Des structures endodontiques complexes à ramifications multiples</li>
            </ul>`
        },
        {
          title: 'Et en pratique, comment faire ?',
          content: `<p>
              Cette impossibilité à atteindre une herméticité radiologique à
              100% doit donc être prise en compte. Plusieurs décisions alors
              sont possibles.
              <br />
              <br />Le patient est adressé à un Endodontiste pour poursuivre
              avec des moyens techniques encore plus spécialisés. (Micro
              chirurgie des racines ou des extrémités des racines sous
              Microscope.)
            </p>
            <p>
              Apres avoir été informé et en l’absence de sensibilité une pause
              est possible. Ce temps de réflexion permet d’évaluer calmement le
              BENEFICE/RISQUE. En effet certaines dents multi traitées ne
              peuvent supporter un démontage de plus sans se fracturer, rendant
              alors l’extraction inévitable.
            </p>`
        },
        {
          title: 'Conclusion',
          content: `<p>
              Les retraitements endodontiques occupent une place importante dans
              l’endodontie quotidienne du praticien dentiste. C’est un acte
              opératoire aux multiples difficultés. Son objectif est d’atteindre
              la zone canalaire apicale afin d’apporter irrigation et
              désinfection et mise en forme avant ré-obturation
              tridimensionnelle étanche. La règle est de « tenter de faire mieux
              » et surtout « essayer de ne pas faire plus mal ».
              <br />
              <br />Il faut savoir choisir l’instrumentation la mieux adaptée,
              en maîtriser parfaitement le fonctionnement et surtout consacrer
              du Temps pour être Disponible et Attentif. Le praticien doit être
              capable d’analyser sa capacité à gérer son acte et d’accepter de
              passer la main si nécessaire.
              <br />
              <br />Le praticien et le patient doivent collaborer pour se donner
              le temps et l’attention qui souvent dénoue des situations pourtant
              complexes.
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
          text: 'Endodontie',
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
