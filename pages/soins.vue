<template>
  <div class="container">
    <div class="full-container">
      <div>
        <h2 class="text-center mt-5">Par Catégorie</h2>
        <hr />
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
      </div>
    </div>

    <div class="text-center">
      <h2>Par question</h2>
      <hr />
      <br />
    </div>
  </div>
</template>

<style scoped lang="scss">
.full-container {
  display: flex;
  justify-content: center;
  // min-height: 72vh;
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
</style>
