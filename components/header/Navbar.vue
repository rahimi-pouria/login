<template>
  <div class="d-flex g24">
    <div v-for="(item, i) in menu" :key="i" class="d-flex">
      <NuxtLink :to="item.path">
        {{ item.name }}
      </NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavbarComponent',
  data () {
    return {
      menu: [
        {
          name: 'خانه',
          path: '/'
        },
        {
          name: 'ورود',
          path: '/Login'
        },
        {
          name: 'ثبت نام',
          path: '/SignUp'
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
