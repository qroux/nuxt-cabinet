<template>
  <div class="full-container">
    <div class="container-fluid">
      <div class="article-bg">
        <h1>Implantologie</h1>
      </div>
    </div>
    <div class="container">
      <div class="full-article">
        <div class="article-content">
          <div class="d-flex justify-content-center align-items-center">
            <h2 class="font-weight-bold">Le recours aux implants, pourquoi et comment ?</h2>
          </div>

          <div>
            <hr />
            <br />
            <br />

            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis, similique. Velit voluptates fuga esse saepe officiis tempora molestias quaerat voluptate eos id! Debitis modi inventore tempore voluptatem nesciunt eaque maiores!</p>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sint ad distinctio dolorum provident voluptate ex velit accusantium ratione quasi libero sapiente eaque temporibus quos molestias totam odit nostrum, vel sequi.</p>
            <br />
            <b-container>
              <b-row class="justify-content-between">
                <b-col cols="12" sm="6" id="implant-A"></b-col>

                <b-col cols="12" sm="6" id="implant-B"></b-col>
              </b-row>
            </b-container>
            <br />
          </div>
          <div class="my-5 py-1" />

          <div class="questions">
            <div class="separator">
              <h2 class="text-center">Questions</h2>
            </div>
            <hr class="mb-5" />
            <div class="d-flex justify-content-start align-items-center">
              <h3 class="dotted" v-b-toggle="'collapse-2'">Dans quels cas recourir aux implants ?</h3>
            </div>

            <b-collapse id="collapse-2">
              <hr />
              <br />
              <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Tempora inventore cupiditate totam deleniti soluta minus, fuga quasi dolore animi reprehenderit, reiciendis delectus amet, praesentium blanditiis aut voluptatibus nam quaerat voluptatem!</p>
              <br />
            </b-collapse>
            <br />

            <div class="d-flex justify-content-start align-items-center">
              <h3
                class="dotted"
                v-b-toggle="'collapse-3'"
              >Quelles sont les alternatives aux implants ?</h3>
            </div>

            <b-collapse id="collapse-3">
              <hr />
              <br />
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Est, in voluptate! Quasi et cum minima deserunt recusandae, laboriosam provident voluptatibus rem, doloremque ab similique ex amet natus? Necessitatibus, assumenda aut.</p>
              <br />
            </b-collapse>
            <br />

            <div class="d-flex justify-content-start align-items-center">
              <h3 class="dotted" v-b-toggle="'collapse-4'">Et en pratique, comment faire ?</h3>
            </div>

            <b-collapse id="collapse-4">
              <hr />
              <br />
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Earum sit iusto laboriosam vero, nihil rem hic quisquam nulla fugit accusamus, enim saepe ipsa consequuntur eligendi itaque nobis nesciunt ratione. Maiores!</p>

              <br />
            </b-collapse>
            <br />

            <div class="d-flex justify-content-start align-items-center">
              <h3 class="dotted" v-b-toggle="'collapse-5'">Conclusion</h3>
            </div>

            <b-collapse id="collapse-5">
              <hr />
              <br />
              <p>
                Cette impossibilité à atteindre une herméticité radiologique à 100%
                doit donc être prise en compte. Plusieurs décisions alors sont
                possibles.
                <br />
                <br />1/ Le patient est adressé à un Endodontiste pour poursuivre avec des
                moyens techniques encore plus spécialisés. (Micro chirurgie des
                racines ou des extrémités des racines sous Microscope.)
              </p>
              <p>
                2/ Apres avoir été informé et en l’absence de sensibilité une pause
                est possible. Ce temps de réflexion permet d’évaluer calmement le
                BENEFICE/RISQUE. En effet certaines dents multi traitées ne peuvent
                supporter un démontage de plus sans se fracturer, rendant alors
                l’extraction inévitable.
              </p>
              <br />
            </b-collapse>
            <br />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

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

.article-content {
  padding: 7vh 0;
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

h3 {
  color: rgba(0, 0, 0, 0.7);
  &:hover {
    cursor: pointer;
    color: rgba(0, 0, 0, 1);
  }
}

.dotted:before {
  content: '\00b7	\00a0	\00a0	\00a0 \00a0';
}
.title {
  color: rgba(0, 0, 0, 0.7);
  font-weight: bold;
}

.main-photo {
  width: 100%;
  height: 200px;
  background-image: url('~assets/implants-radio.jpg');
  background-position: center;
  background-size: cover;
}

#implant-A,
#implant-B {
  height: 15vh;
  background-position: center;
  background-size: cover;
}

#implant-A {
  background-image: url('~assets/implants-radio-A.jpg');
}

#implant-B {
  background-image: url('~assets/implants-radio-B.jpg');
}

.questions {
}

.separator {
  background-color: #262b36;
  color: white;
  padding: 5px 0;
}
</style>
