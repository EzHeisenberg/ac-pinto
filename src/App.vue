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


html, body
  margin: 0
  padding: 0
  border: 0
  min-height: 100vh
  background-color: #fff


.container
  padding: $padding-container-desktop


h1, h2, h3, h4, h5, h6
  margin: 0


.big-title
  font-family: $font-title
  font-size: $size-big-title-desktop
  padding-top: 20px


.title
  font-family: $font-title
  font-size: $size-title-desktop
  padding-bottom: 20px


.subtitle
  font-family: $font-paragraph-regular
  font-size: $size-subtitle-desktop
  padding: 15px 0

.paragraph-regular
  font-family: $font-paragraph-regular
  font-size: $size-paragraphe-desktop


.paragraph-bold
  font-family: $font-paragraph-bold
  font-size: $size-paragraphe-desktop


.bottom-bar
  border-bottom: 4px solid
  box-shadow: 5px 5px 5px rgba(85, 85, 85, 0.18)
  margin-bottom: 30px

.c-white
  color: $colors-white

.c-black
  color: $colors-black

.c-yellow
  color: $colors-yellow

.c-red
  color: $colors-red

.c-silver
  color: $colors-silver

.w5
  width: 5%
.w10
  width: 10%
.w15
  width: 15%
.w20
  width: 20%




@media screen and (max-width: 900px)



@media screen and (max-width: 700px)
  .container
    padding: $padding-container-pad


  .big-title
    font-size: $size-big-title-pad

  .title
    font-size: $size-title-pad

  .subtitle
    font-size: $size-subtitle-pad

  .paragraph-regular .paragraph-bold
    font-size: $size-paragraphe-pad



@media screen and (max-width: 480px)
  .container
    padding: $padding-container-mobile


@media screen and (max-width: 375px)



</style>