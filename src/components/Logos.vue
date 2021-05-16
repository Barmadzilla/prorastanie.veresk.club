<template>
  <div class="content">
    <div>
      <h3>Валерий и Юлия Казас</h3>
      <h4>Ленд-арт</h4>
    </div>
    <div class="logo">
      <a href="#"><img src="../assets/images/logos/logo-sparta.svg" alt=""></a>
      <a href="https://veresk.club"><img src="../assets/images/logos/logo-veresk.svg" alt=""></a>
    </div>

  </div>
</template>

<script>
export default {
  name: "Logos"
}
</script>

<style scoped>
h3, h4 {
  font-weight: normal;
  text-transform: uppercase;
}

h3 {
  font-size: 2.5em;
}

h4 {
  font-size: 1.5em;
}

.content,
.logo {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  align-items: flex-end;
}

.logo a {
  margin-left: 3em;
}

@media (max-width: 800px) {
  .content {
    flex-direction: column;
  }

  h3, h4 {
    text-align: center;
  }

  .logo {
    margin-top: 2em;
  }

  .logo a {
    margin: 1em;

  }

  .logo a img {
    max-height: 5em;
  }
}
@media (max-width: 420px){
  h3 {
    font-size: 1.5em;
  }

  h4 {
    font-size: 1em;
  }
  .logo a img {
    max-width: 25vw;
  }
  .logo {
    margin-top: unset;
    align-items: center;
  }
}
</style>