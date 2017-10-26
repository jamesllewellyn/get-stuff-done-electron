<template>
  <!--<div class="hero-body">-->
    <!--<div class="container">-->
      <div id="app">
        <router-view></router-view>
      </div>
    <!--</div>-->
  <!--</div>-->
</template>

<script>
  export default {
    name: 'get-stuff-done-electron'
  }
</script>

<style lang="scss">
    @import url(//fonts.googleapis.com/css?family=Raleway:300,400,600);
    @import "./node_modules/bulma/bulma";
    @import "assets/sass/variables";
    @import "assets/sass/transitions";
    /*!** main App Structure *!*/
    @import "assets/sass/structure";
    @import "assets/sass/forms";
    @import "assets/sass/typography";
    @import "assets/sass/buttons";
    @import "assets/sass/tables";
</style>
