<template>
  <section>
    <div class="img animate__animated animate__fadeInLeft"></div>
    <article class="animate__animated animate__fadeInRight">
      <h2>The leader in interactive VR</h2>
      <p>
        Founded in 2011, Loopstudios has been producing world-class virtual
        reality projects for some of the best companies around the globe. Our
        award-winning creations have transformed businesses through digital
        experiences that bind to their brand.
      </p>
    </article>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
section {
  display: flex;
  flex-direction: column;
  padding: 4rem 2rem;
  align-items: center;
  justify-content: center;
  text-align: center;
  gap: 2rem;
}
.img {
  width: 100%;
  background-image: url("../assets/mobile/image-interactive.jpg");
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover;
  min-height: 20rem;
  z-index: 5;
}

article {
  display: flex;
  flex-direction: column;
  padding: 0 2rem;
  gap: 1rem;
  background: hsl(0, 0%, 100%);
  z-index: 5;
}

@media (min-width: 1200px) {
  section {
    flex-direction: row;
    position: relative;
    height: 100vh;
  }
  .img {
    position: absolute;
    background-image: url("../assets/desktop/image-interactive.jpg");
    background-position: center center;
    top: 5rem;
    left: 8rem;
    bottom: 10rem;
    max-width: 50rem;
    box-shadow: rgba(60, 64, 67, 0.3) 0px 1px 2px 0px,
      rgba(60, 64, 67, 0.15) 0px 1px 3px 1px;
  }
  article {
    position: absolute;
    bottom: 5rem;
    right: 8rem;
    left: 50%;
    padding: 4rem 3.65rem;
    box-shadow: rgba(60, 64, 67, 0.3) 0px 1px 2px 0px,
      rgba(60, 64, 67, 0.15) 0px 1px 3px 1px;
  }
  p {
    text-align: left;
  }
}
</style>
