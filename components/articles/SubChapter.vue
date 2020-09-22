<template>
  <div>
    <div class="d-flex justify-content-start">
      <h7>
        <b-icon-chevron-compact-down />
      </h7>
      <h3 v-b-toggle="`collapse-${num}`" class="icon-margin">{{title}}</h3>
    </div>

    <b-collapse :id="`collapse-${num}`">
      <hr />
      <br />
      <slot name="content"></slot>
      <br />
    </b-collapse>
  </div>
</template>

<script>
import { BIconChevronCompactDown } from 'bootstrap-vue'

export default {
  props: ['title', 'num'],
  components: {
    BIconChevronCompactDown
  }
}
</script>



<style scoped lang="scss">
$animate: all 0.2s ease-in-out;

.icon-margin {
  margin-left: 2vw;
  &:focus {
    outline: none;
  }
}

@media screen and (max-width: 768px) {
  h1 {
    font-size: 30px;
  }
  h3 {
    font-size: 25px;
  }
  .icon-margin {
    margin-left: 5vw;
  }
}
</style>
