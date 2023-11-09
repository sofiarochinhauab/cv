<template>
  <footer>

    <a class="" href="https://www.facebook.com/">
      <img alt="Vue logo" src="../assets/icon-facebook.png" height="50" />
    </a>
    <a href="https://www.instagram.com/">
      <img alt="Vue logo" src="../assets/icon-instagram.png" height="50" />
    </a>
    <a href="https://www.tiktok.com/">
      <img alt="Vue logo" src="../assets/icon-tiktok.png" height="50" />
    </a>
    <p>Copyright &copy; {{ year }}</p>
  </footer>

</template>

<style>
footer {
  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
  text-align: center;
  display: flex;

  p {
    float: right;
  }
}


</style>
<script>
import { computed } from "vue";

export default {
  setup() {
    const year = computed(() => new Date().getFullYear());
    return { year };
  },
};
</script>
