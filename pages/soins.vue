<template>
  <div class="container full-container">
    <b-tabs class="mt-5 full-tab" content-class="mt-5" fill>
      <b-tab title="Par Catégorie" active>
        <b-card-group deck class="pb-5">
          <b-card
            tag="nuxt-link"
            to="/implantologie"
            title="Implantologie"
            img-src="~/assets/implantologie.jpg"
            img-alt="Image"
            img-top
          ></b-card>

          <b-card
            tag="nuxt-link"
            to="/parodontologie"
            title="Parodontologie"
            img-src="~/assets/paro.jpg"
            img-alt="Image"
            img-top
          ></b-card>

          <b-card
            tag="nuxt-link"
            to="/endodontie"
            title="Endodontie"
            img-src="~/assets/prevention.jpg"
            img-alt="Image"
            img-top
          ></b-card>
        </b-card-group>
      </b-tab>
      <b-tab title="Par Question">
        <div v-for="question in questions">
          <nuxt-link :to="question.link">
            <h3>{{ question.title}}</h3>
          </nuxt-link>
        </div>
      </b-tab>
    </b-tabs>
    <!-- <div class="full-container">
      <div>
        <div class="d-flex justify-content-start align-items-center">
          <h2 block v-b-toggle.accordion-1 class="mt-5">Par Catégorie</h2>
          <div class="mt-5 mx-3">
            <h3>/</h3>
          </div>
          <h2 block v-b-toggle.accordion-2 class="mt-5">Question</h2>
        </div>

        <hr />

        <b-collapse id="accordion-1" visible accordion="my-accordion">
          <b-card-group deck class="py-5">
            <b-card
              tag="nuxt-link"
              to="/implantologie"
              title="Implantologie"
              img-src="~/assets/implantologie.jpg"
              img-alt="Image"
              img-top
            ></b-card>

            <b-card
              tag="nuxt-link"
              to="/parodontologie"
              title="Parodontologie"
              img-src="~/assets/paro.jpg"
              img-alt="Image"
              img-top
            ></b-card>

            <b-card
              tag="nuxt-link"
              to="/endodontie"
              title="Endodontie"
              img-src="~/assets/prevention.jpg"
              img-alt="Image"
              img-top
            ></b-card>
          </b-card-group>
        </b-collapse>
      </div>
    </div>

    <div class="pb-5">
      <br />
      <b-collapse id="accordion-2" accordion="my-accordion" v-for="question in questions">
        <nuxt-link :to="question.link">
          <h5>{{ question.title}}</h5>
        </nuxt-link>
      </b-collapse>
    </div>-->
  </div>
</template>

<script>
export default {
  props: {
    questions: {
      default: () => [
        {
          title: 'Comment traiter un saignement de gencive ?',
          link: '/endodontie'
        },
        {
          title:
            'Je pense avoir une carie, ma dent va-t-elle être dévitalisée ?',
          link: '/endodontie'
        },
        {
          title:
            "Ma dent a été dévitalisée, la pose d'une couronne est-elle nécessaire ?",
          link: '/endodontie'
        },
        {
          title: 'Je suis phobique, comment me faire soigner ?',
          link: '/endodontie'
        },

        {
          title: 'Mon traitement de racine a échoué, ma dent est-elle perdue ?',
          link: '/endodontie'
        },
        {
          title: 'Mes dents sont usées, que faire pour les préserver ?',
          link: '/endodontie'
        },
        {
          title: 'Mes racines sont apparentes, que faire ?',
          link: '/parodontologie'
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
</style>
