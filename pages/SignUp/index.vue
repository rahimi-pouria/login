<template>
  <div class="d-flex bg-DarkBlue Login w-100">
    <div class="d-flex container pt-4 flex-wrap">
      <div class="col-md-6 col-sm-12"></div>
      <div class="col-md-6 col-sm-12">
        <div class="d-flex g16 flex-wrap w-100">
          <!--   text login       -->
          <div class="d-flex flex-column g18 pt-4">
            <p class="f14-400">SANAM - FavaMajd Cooperation</p>
            <p class="f14-400">Remote Desktop and App Solutions</p>
            <p class="f14-400">Copyright 2014 - 2023</p>
            <p class="f14-400">Last Login:  Status: OK / Failed </p>
          </div>
          <!--  form login        -->
          <div class="d-flex w-50 g16 flex-column form">
            <input type="text" placeholder="userName" class="form-control">
            <input type="email" placeholder="email" class="form-control">
            <input type="password" placeholder="password" class="form-control">
            <div class="d-flex g8">
              <button class="bg-warning px-4 border-0 py-1 r-6" style="width: 45% !important">
                sign up
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
  name: 'index.vue',
  layout: 'Default'
}
</script>

<style scoped>
.Login{
  color: #ffffff !important;
  height: 80vh;
}
</style>
