<template>
  <div class="about">
    <div class="flex flex-row justify-center items-center h-about bg-black">
      <div class="w-3/6 mr-5">
        <h1 class="text-2xl font-bold text-white">
          Je suis un étudiant de 20 ans à l'EEMI, l'École des Métiers d'Internet, en Bachelor Chef de Projets Digitaux, spécialisation Web Development.<br><br>
          Fort d'une passion pour l'informatique depuis tout petit, et avec de
          l'expérience, notamment chez LDLC et Qwant, c'est tout naturellement que je
          me suis orienté vers le métier de développeur web. Un domaine autodidacte
          et stimulant, qui me permet d'aider les gens via mon travail.
        </h1>
      </div>
      <div class="w-1/5 ml-3 bg-green-300">
        <img src="../assets/img/hibiki.jpg" alt="">
      </div>
    </div>
    <div class="h-96">
      <h2>test</h2>
      <img src="../assets/img/github.svg" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name: 'About'
}
</script>

<style scoped lang="scss">
  .h-about {
    height: 45vh;
  }
</style>
