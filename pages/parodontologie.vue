<template>
  <div class="full-container">
    <div class="container-fluid">
      <div class="article-bg">
        <h1>Parodontologie</h1>
      </div>
    </div>
    <div class="container">
      <div class="full-article">
        <div class="article-content py-5">
          <section></section>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
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
  background-image: linear-gradient(rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.3)),
    url('~assets/paro.jpg') !important;
  text-align: center;
  background-image: url('~assets/paro.jpg');
  background-size: cover;
  background-position: center;
}
.full-article {
  display: flex;
  flex-direction: column;
}
</style>
