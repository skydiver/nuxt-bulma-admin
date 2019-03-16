<template>
  <div>
    <NavBar />
    <div class="container">
      <div class="columns">
        <div class="column is-3 ">
          <SideBar />
        </div>
        <div class="column is-9">
          <div class="columns">
            <div class="column is-12">
              <nuxt />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NavBar from '~/components/NavBar.vue'
import SideBar from '~/components/SideBar.vue'

export default {
  components: {
    NavBar,
    SideBar
  }
}
</script>

<style>
html,
body {
  font-family: 'Open Sans', serif;
  font-size: 16px;
  line-height: 1.5;
  height: 100%;
  background: #ecf0f3;
}
.columns {
  width: 100%;
  height: 100%;
  margin-left: 0;
}
</style>
