<template>
  <div class="full-container">
    <div class="container-fluid">
      <div class="article-bg">
        <h2>Dentophobie</h2>
      </div>
    </div>
    <b-breadcrumb :items="items"></b-breadcrumb>
    <div class="container">
      <div class="full-article">
        <div class="article-content">
          <div class="header pt-3 pb-3">
            <h1 class="title">J'ai peur d'aller chez le dentiste, comment me faire soigner ?</h1>
            <hr />
          </div>

          <b-container class="my-4">
            <b-row>
              <b-col cols="12">
                <p>
                  Certains se sentent stressés à l’idée même de se rendre chez le dentiste.On estime à 30% ceux qui avoue le conflit intérieur qu’ils ressentent avant de pouvoir prendre un rendez vous.
                  <br />
                  <strong>Un vécu traumatisant au cours de l’enfance, lors de mauvaises expériences, est souvent à l’origine de cette phobie.</strong> Elle se manifeste sur le fauteuil dentaire par des accélérations du coeur, de la transpiration mais cet état est souvent précédé d’insomnies la veille même du rendez vous.
                </p>

                <p>
                  La dentophobie apparait comme une peur primitive semblant irrationnelle.
                  Malgré tous les progrès techniques et leurs promesses pour “Ne pas avoir mal”, le phobique ne se sent pas rassuré, et bien souvent pas du tout pris au sérieux face à “sa peur à lui”.
                  Ce conflit non résolu et cette impasse dans le refus des soins, sont extrêment dommageables, aussi bien pour l'état dentaire que l’état général et psychique.
                  <strong>L’aide professionnelle prévenante et structurée peut organiser efficacement la sortie de cette impasse.</strong>
                </p>
                <p>
                  <strong>Notre objectif central est d’enlever la peur du dentiste palier par palier pour permettre aux patients phobiques de reprendre contrôle et reprendre leur souffle.</strong> Construire un rapport de confiance clair est fondamental.
                </p>
                <p>
                  La démarche d'accompagnement est étagée grâce à l’utilisation de différentes procédures comme le protoxyde d’azote, les traitements tranquillisants ou sédatifs voir même dans certain cas l'anesthésie générale.
                  <strong>En fin de traitement, l'assainissement dentaire doit être atteint mais, au delà, l'objectif est l’autonomie du patient pour poursuivre ses traitements en toute normalité et sans anxiété.</strong>
                </p>
              </b-col>
            </b-row>
          </b-container>
          <br />

          <!-- <div class="d-flex justify-content-start align-items-center">
          </div>-->

          <b-container>
            <h2 class="font-weight-bold mb-4">Le traitement des patients phobiques</h2>

            <div class>
              <h3 v-b-toggle="'collapse-1'" class="dotted mb-2">Mise en confiance</h3>
              <b-collapse id="collapse-1" visible>
                <br />
                <p>
                  <strong>Le passé des phobiques est majoritairement cristallisé sur une rupture de confiance.</strong> Un traitement subit par un dentiste autoritaire et brutal. Une promesse rapide de ne pas faire mal, mais non tenue. Une sensation de faiblesse face à une autorité parentale liguée à l’action subie de la part du dentiste. Une confusion entre la propre peur des parents muée en autorité et injonction envers l’enfant, prié de croire que le dentiste ne fait pas mal que tout va bien, tout est normal.
                </p>
                <p>
                  <strong>Il est clair qu’un projet dentaire pour un patient anxieux ne peut se construire sans que le patient ait une confiance absolue en son dentiste.</strong> Il attend bien sur un travail bien fait mais aussi d'être informé des étapes de ce travail avenir des moments de repos. Il attend que le dentiste ait l’attention voulue pour lui permettre de marcher à son rythme sans s'essouffler et qu’ils soit conscient de l’anxiété qu’il ressent.
                  Dans le contexte traditionnel des cabinets dentaire ceci est un vrai défi pour le dentiste soumis lui même à son propre stress dans le rythme quotidien débordé.
                </p>
              </b-collapse>
            </div>

            <div class>
              <h3
                v-b-toggle="'collapse-2'"
                class="dotted mb-2"
              >Neutralisation des stimuli anxiogènes</h3>
              <b-collapse id="collapse-2">
                <br />
                <p>
                  Pour un patient phobique, et consécutivement aux expériences faites dans le passé, le cabinet dentaire est un lieu à risques.
                  <br />
                  <strong>En effet cet environnement rassemble un ensemble de signaux auquel il est conditionné négativement.</strong> Un patient phobique a mémorisé et associé émotionnellement des éléments qui agissent même à très faible dose à la manière des allergènes chez des allergiques. Il faudra donc commencer par repérer pour diminuer à minima le nombre et le niveau de ces stimulations perçue négativement.
                </p>
                <p>
                  Un certain nombre de précautions seront donc à prendre.
                  <br />La perception de lumière et d’espace joue favorablement dans les environnements dentaires.
                  Il en va de même les éléments de décoration apportant des touches colorées et vivantes.
                  <strong>Ceci évite aux anxieux la sensation d'étouffement et augmente leur sentiment positif de contrôle et de liberté.</strong>
                  <br />
                  <strong>Le salon d’attente doit assurer un agrément et un confort acoustique</strong> le mettant à l’abris des nuisances sonores désagréables comme le bruit des turbines et des moteurs.
                  <strong>Les attentes doivent être courtes et agréables.</strong> Elles peuvent même être constructives et objets positifs de découverte en matière musicale vidéo ou lecture. Tout ceci peut libérer l’esprit en invitant au voyage.
                </p>
              </b-collapse>
            </div>

            <div class>
              <h3 v-b-toggle="'collapse-3'" class="dotted mb-2">Traitement doux, sans stress</h3>
              <b-collapse id="collapse-3">
                <br />
                <p>
                  <strong>La confiance en le dentiste, la personnalisation des procédures d'anesthésie et le choix technique de matériel ou de produit sont un ensemble cohérent qui doit bénéficier aujourd’hui à tous les patient et à l'évidence tout particulièrement au patients anxieux.</strong>
                </p>
                <p>
                  La crainte d’une anesthésie qui ne “marche pas” est dans ces conditions d’attention non cliniquement fondée.
                  La peur des piqûres chez les patients phobiques nécessite d'être réalisée avec beaucoup de précautions par des “équipes dentiste-assistante” très bien formées et en bonne entente.
                </p>
                <p>Pour atténuer l’inconfort de l’aiguille le protocole mise en place est le suivant :</p>
                <ul>
                  <li>
                    <strong>Préparation du site d’injection par application au coton tige de gel anesthésique de contact.</strong>
                  </li>
                  <li>
                    <strong>Utilisation d'aiguilles très fines 0.27 mm</strong>
                  </li>
                  <li>
                    <strong>Anesthésie intraligamentaire :</strong> l’injection est réalisée avec très peu d’inconfort car la zone est pré-anesthésiée par le gel de contact. L’injection très progressive et très lente est localisée dans l’espace entre la dent et la racine.
                    <strong>Sa diffusion est très rapide et très efficace sans donner un sensation d’engourdissement</strong> très large atteignant les lèvres et la langue.
                  </li>
                </ul>
                <p>
                  <strong>Une surveillance attentive doit déterminer le moment des pauses pour reprendre son souffle et écouter le retour d'information du patient.</strong> Celui-ci est fondamental car il assure un avancement du traitement validé en permanence par l'équilibre émotionnel du patient.
                </p>

                <p>
                  Ce type prévenante d’approche anesthésique, très efficace dans les contextes de faible stress, est néanmoins insuffisante chez dent patient dont la dentophobie est sèvre.
                  <br />
                  <strong>Il existe alors des solutions intermédiaires avant le recours à une anesthésie générale : La sédation consciente au protoxyde d’azote (MEOPA) ou des tranquilisant sont à envisager préalablement et de façon complémentaire.</strong>
                </p>
              </b-collapse>
            </div>
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
          text: 'Dentophobie',
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

#endo1 {
  justify-content: space-around;
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

  #endo1 {
    flex-direction: column !important;
    img {
      margin: 3px 20px;
      border: 1px solid black;
    }
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

  color: rgba(0, 0, 0, 0.5);
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
