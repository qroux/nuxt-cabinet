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
      <b-tab class="mb-5" active>
        <template v-slot:title>
          <h3>Questions</h3>
        </template>
        <div v-for="question in questions" class="py-2">
          <nuxt-link :to="question.link" class="questions">
            <h5>{{ question.title}}</h5>
          </nuxt-link>
        </div>
      </b-tab>
    </b-tabs>
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
</style>
