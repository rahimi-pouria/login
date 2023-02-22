<template>
  <div class="d-flex bg-DarkBlue Login w-100">
    <div class="d-flex container pt-4 flex-wrap">
      <div class="col-md-6 col-sm-12" />
      <div class="col-md-6 col-sm-12">
        <div class="d-flex g16 flex-wrap w-100">
          <!--   text login       -->
          <div class="d-flex flex-column g18 pt-4">
            <p class="f14-400">
              SANAM - FavaMajd Cooperation
            </p>
            <p class="f14-400">
              Remote Desktop and App Solutions
            </p>
            <p class="f14-400">
              Copyright 2014 - 2023
            </p>
            <p class="f14-400">
              Last Login:  Status: OK / Failed
            </p>
          </div>
          <!--  form login        -->
          <div class="d-flex w-50 g16 flex-column form">
            <input v-model="userName" type="text" placeholder="userName" class="form-control">
            <input v-model="password" type="password" placeholder="password" class="form-control">
            <div class="d-flex g8">
              <button
                class="bg-warning px-4 border-0 py-1 r-6"
                style="width: 45% !important"
                @click="Login"
              >
                Login
              </button>
              <select class="form-control w-50">
                <option>English</option>
                <option>Persian</option>
              </select>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  layout: 'Default',
  data () {
    return {
      userName: '',
      password: null
    }
  },
  methods: {
    Login () {
      fetch('https://dummyjson.com/auth/login', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify({
          username: 'kminchelle',
          password: '0lelplR'
        })
      })

        .then(res => res.json())
      this.$router.push('/Profile')
    }
  }
}
</script>

<style scoped>
  .Login{
    color: #ffffff !important;
    height: 80vh;
  }
</style>
