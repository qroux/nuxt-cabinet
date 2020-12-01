<template>
  <div class="full-container">
    <div class="container-fluid">
      <div class="article-bg">
        <h1>Prévention</h1>
      </div>
    </div>
    <div class="container">
      <div class="full-article">
        <div class="article-content py-5">
          <h2>Description</h2>
          <hr />
          <b-icon-chevron-compact-down />
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatum
            fugiat non aut quos numquam nemo sapiente, earum deserunt! Nobis
            quod repellat fuga inventore ad blanditiis beatae, ipsam eveniet,
            ullam quo.
          </p>
          <h2>Indications / Contre-Indications</h2>
          <hr />
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatum
            fugiat non aut quos numquam nemo sapiente, earum deserunt! Nobis
            quod repellat fuga inventore ad blanditiis beatae, ipsam eveniet,
            ullam quo.
          </p>
          <h2>Plan De Traitement</h2>
          <hr />
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatum
            fugiat non aut quos numquam nemo sapiente, earum deserunt! Nobis
            quod repellat fuga inventore ad blanditiis beatae, ipsam eveniet,
            ullam quo.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { BIconChevronCompactDown } from 'bootstrap-vue'

export default {
  components: {
    BIconChevronCompactDown
  }
}
</script>  

<style scoped lang="scss">
.full-container {
  min-height: 73vh;
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
  background-image: url('~assets/prevention.jpg');
  background-size: cover;
}
.full-article {
  display: flex;
  flex-direction: column;
}
</style>
