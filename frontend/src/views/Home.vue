<template>
  <div class="main">
    <h1>Welcome to the {{ projectName }} {{ projectVersion }} application</h1>
    <h4>Start by choosing one of the elements on the top menu</h4>
  </div>
</template>

<script>
export default {
  name: 'Home',
  data () {
    return {
      projectName: process.env.VUE_APP_PROJECT_TITLE,
      projectVersion: `[${config.VUE_APP_PROJECT_VERSION}]` || ''
    }
  }
}
</script>

<style lang="scss" scoped>
div.main {
  text-align: center;
  margin-top: 25px;
}
</style>
