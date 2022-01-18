<template>
  <div class="boxes d-flex justify-center align-center flex-lg-row flex-md-row" v-if="showHome">
    <RouterLink :to="{name: 'About'}"><img @click="clicked" src="../images/second-box.png" alt="Images" width="400" class="">
    </RouterLink>
    <img src="../images/second-box.png" alt="Images" width="400" class="ml-lg-3">
    <img src="../images/second-box.png" alt="Images" width="400" class="ml-lg-3">
  </div>
</template>

<script>
export default {
  name: 'Boxes',
  data() {
    return {
      showHome: true
    }
  },
  methods: {
    clicked() {

    }
  }
}
</script>

<style scoped>
.boxes {
  background: #159957;
  background: -webkit-linear-gradient(to right, #155799, #159957);
  background: linear-gradient(to right, #155799, #159957);
  min-height: 100vh;

}

img:hover {
  transform: rotate(10deg);
  transition: 500ms ease;
  animation: animate-dialog 300ms infinite forwards running;
  cursor: pointer;
}

@keyframes animate-dialog {
  0% {
    transform: translate(0);
  }
  50% {
    transform: rotate(-4deg);
  }
  100% {
    transform: rotate(4deg);
  }
}

@media (max-width: 1250px) {
  img {
    width: 300px;
  }
}

@media (max-width: 900px) {
  img {
    width: 200px;
  }
}

@media (max-width: 650px) {
  .boxes {
    flex-direction: column;
  }
}
</style>