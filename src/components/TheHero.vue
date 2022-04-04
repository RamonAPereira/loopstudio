<template>
  <section>
    <div class="animate__animated animate__fadeInLeft">
      <h1>Immersive Experiences that deliver</h1>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
section {
  align-items: center;
  background-image: url("../assets/mobile/image-hero.jpg");
  background-repeat: no-repeat;
  background-position: center center;
  background-size: cover;
  display: flex;
  height: 100vh;
  widows: 100vw;
  justify-content: center;
}

div {
  border: 2px hsl(0, 0%, 100%) solid;
  padding: 1rem;
  max-width: 20rem;
}

h1 {
  color: hsl(0, 0%, 100%);
  font-size: 2.5rem;
}

@media (min-width: 800px) {
  section {
    justify-content: left;
    padding: 8rem;
    background-image: url("../assets/desktop/image-hero.jpg");
    background-repeat: no-repeat;
    background-position: center center;
    background-size: cover;
  }
  div {
    max-width: 35rem;
    padding: 2rem;
  }
  h1 {
    font-size: 3.5rem;
  }
}
</style>
