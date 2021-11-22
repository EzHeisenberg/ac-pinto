<template>
  <div class="undulate-container">

    <svg class="svg-head" viewBox="0 0 1440 128" xmlns="http://www.w3.org/2000/svg">
      <g>
        <path stroke="null" id="svg_1"
              d="m0,0l80,0c80,0 240,0 400,42.7c160,42.3 321.67654,84.71008 481.67654,84.41008c160,0.3 318.32346,-42.11008 398.32346,-84.41008l80,-42.7l0,256l-80,0c-80,0 -240,0 -400,0c-160,0 -320,0 -480,0c-160,0 -320,0 -400,0l-80,0l0,-256z"
              fill="#531B26"/>
      </g>
    </svg>

    <div class="container">

      <h3 class="title c-yellow">Travaux neufs ou travaux de rénovation</h3>
      <div class="bottom-bar c-yellow w20"></div>

      <ul class="jobs-container c-silver">
        <li class="jobs-list subtitle">Carrelage sol, mur, intérieur et extérieur</li>
        <li class="jobs-list subtitle">Pose de pierre</li>
        <li class="jobs-list subtitle">Revêtement de sol souple</li>
        <li class="jobs-list subtitle">Moquette</li>
        <li class="jobs-list subtitle">Placoplâtre mur et plafond</li>
        <li class="jobs-list subtitle">Parquets massif, stratifié clipser, flottant</li>
      </ul>

      <div class="logo-container">
        <img :src="require(`@/assets/Accueil/acpintologo.png`)" alt="logo AC Pinto">
      </div>
    </div>

    <svg class="svg-foot" viewBox="0 0 1440 128" xmlns="http://www.w3.org/2000/svg">
      <g>
        <path stroke="null" id="svg_1"
              d="m0,0l80,0c80,0 240,0 400,42.7c160,42.3 321.67654,84.71008 481.67654,84.41008c160,0.3 318.32346,-42.11008 398.32346,-84.41008l80,-42.7l0,256l-80,0c-80,0 -240,0 -400,0c-160,0 -320,0 -480,0c-160,0 -320,0 -400,0l-80,0l0,-256z"
              fill="#FFFFFF"/>
      </g>
    </svg>

  </div>
</template>

<script>
export default {
  name: "wave-container"
}
</script>


<style lang="sass" scoped>
@import "../../styles/variables"


.undulate-container
  background: $colors-red

.svg-head
  background: #FFFFFF
  margin: 0
  display: block

.svg-foot
  margin: 0
  display: block


.jobs-container
  padding: 5px 50px
  list-style: circle

  li
    padding: 10px


.logo-container
  position: fixed
  right: $padding-container-desktop
  bottom: 25px
  img
    height: 300px



@media screen and (max-width: 900px)
  .logo-container
    bottom: 100px
    img
      height: 180px

@media screen and (max-width: 700px)
  .logo-container
    display: none


@media screen and (max-width: 480px)


@media screen and (max-width: 375px)


</style>