<template>
  <div class="d-flex flex-column">
    <div class="d-flex header w-100">
      <header-component class="text-white" />
    </div>
    <div class="d-flex">
      <Nuxt />
    </div>
  </div>
</template>

<script>
import HeaderComponent from '~/components/Header.vue'

export default {
  name: 'Default',
  components: { HeaderComponent }
}
</script>

<style scoped>
.header{
  background: url("@/assets/img/login-head-img.png");
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  color: #ffffff !important;
  padding: 120px;
  justify-content: center;
  align-items: center;
}
</style>
