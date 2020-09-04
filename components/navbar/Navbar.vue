<template>
  <div>
    <b-navbar toggleable="lg" type="light">
      <nuxt-link to="/">
        <img id="logo" src="~/assets/dental-logo.png" />
      </nuxt-link>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-3">
          <nuxt-link id="custom-links" to="cabinet">Le Cabinet</nuxt-link>
          <nuxt-link id="custom-links" to="soins">Les Soins</nuxt-link>
          <nuxt-link id="custom-links" to="info">Infos Pratiques</nuxt-link>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script></script>

<style scoped lang="scss">
#logo {
  height: 5vh;
  width: auto;
}
.navbar {
  border-bottom: 1px solid white;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
  background-color: #262b36;
  .navbar-brand {
    font-size: 32px !important;
    margin: 0 2vw;
  }
  .navbar-nav {
    align-items: center;
    font-size: 22px;
  }
}
#custom-links {
  text-decoration: none;
  color: rgba(255, 255, 255, 0.5);
  margin: 0 1vw;
  &:hover {
    color: rgba(255, 255, 255, 0.8);
  }
}
</style>
