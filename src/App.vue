<template>
  <div id="app">
    <Navigation></Navigation>
    <router-view/>







  </div>
</template>



<script>
// @ is an alias to /src
import Navigation from '@/components/Navigation.vue'

export default {
  components: {
    Navigation,
  }
}
</script>



<style lang="sass">
@import "styles/variables.sass"


@font-face
  font-family: "Eurostyle"
  src: url("styles/fonts/Eurostyle.ttf") format("truetype")

@font-face
  font-family: "ObjektivMk2W03-Bold"
  src: url("styles/fonts/Objektiv Mk2 W03 Bold.ttf") format("truetype")

@font-face
  font-family: "ObjektivMk2W03-Light"
  src: url("styles/fonts/Objektiv Mk2 W03 Regular.ttf") format("truetype")


body
  margin: 0
  padding: 0
  min-height: 100vh
  background-color: $colors-yellow

.container
  padding: 0 20px


h1, h2, h3, h4, h5, h6
  margin: 0


.big-title
  font-family: $font-title
  font-size: $size-big-title
  padding-top: 20px


.title
  font-family: $font-title
  font-size: $size-title



.subtitle
  font-family: $font-paragraph-regular
  font-size: $size-subtitle
  padding-top: 10px





.c-white
  color: $colors-white

.c-black
  color: $colors-black


</style>