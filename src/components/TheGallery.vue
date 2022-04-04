<template>
  <section>
    <h2>Our Creations</h2>
    <ul>
      <li class="deep-earth animate__animated animate__fadeIn">
        <strong>Deep Earth</strong>
      </li>
      <li class="night-arcade animate__animated animate__fadeIn">
        <strong>Night Arcade</strong>
      </li>
      <li class="soccer-team animate__animated animate__fadeIn">
        <strong>Soccer Team VR</strong>
      </li>
      <li class="the-grid animate__animated animate__fadeIn">
        <strong>The Grid</strong>
      </li>
      <li class="from-up the-grid animate__animated animate__fadeIn">
        <strong>From Up Above VR</strong>
      </li>
      <li class="pocket-borealis the-grid animate__animated animate__fadeIn">
        <strong>Pocket Borealis</strong>
      </li>
      <li class="the-curiosity the-grid animate__animated animate__fadeIn">
        <strong>The Curiosity</strong>
      </li>
      <li class="make-fisheye the-grid animate__animated animate__fadeIn">
        <strong>Make It Fisheye</strong>
      </li>
    </ul>
    <a href="#">See All</a>
  </section>
</template>

<style scoped>
section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  gap: 2rem;
}
a {
  text-align: center;
  text-decoration: none;
  text-transform: uppercase;
  padding: 1rem 2rem;
  border: 1px solid hsl(0, 0%, 0%);
  max-width: fit-content;
  margin: 0 auto;
  color: hsl(0, 0%, 0%);
}
a:hover {
  background: hsl(0, 0%, 0%);
  color: hsl(0, 0%, 100%);
  transition: all 0.3s ease-in;
}

h2 {
  text-align: center;
}
ul {
  display: grid;
  gap: 1rem;
  color: hsl(0, 0%, 100%);
  padding: 0 2rem;
}

li {
  position: relative;
  display: flex;
  align-items: flex-end;
  justify-content: left;
  padding: 0.5rem;
  background-position: bottom bottom;
  background-size: cover;
  background-repeat: no-repeat;
  min-height: 8rem;
  background-blend-mode: saturation;
}
li::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  background: rgba(000, 000, 000, 0.5);
  z-index: 5;
}
li:hover {
  color: hsl(0, 0%, 0%);
  transition: all 0.2s ease-in;
}
li:hover::before {
  background: hsla(0, 0%, 55%, 0.8);
  cursor: pointer;
  transition: all 0.2s ease-in;
}

strong {
  display: block;
  font-size: 1.5rem;
  max-width: 10rem;
  z-index: 10;
}
.deep-earth {
  background-image: url("../assets/mobile/image-deep-earth.jpg");
}
.night-arcade {
  background-image: url("../assets/mobile/image-night-arcade.jpg");
}
.soccer-team {
  background-image: url("../assets/mobile/image-soccer-team.jpg");
}
.deep-earth {
  background-image: url("../assets/mobile/image-deep-earth.jpg");
}
.the-grid {
  background-image: url("../assets/mobile/image-grid.jpg");
}
.from-up {
  background-image: url("../assets/mobile/image-from-above.jpg");
}
.pocket-borealis {
  background-image: url("../assets/mobile/image-pocket-borealis.jpg");
}
.the-curiosity {
  background-image: url("../assets/mobile/image-curiosity.jpg");
}
.make-fisheye {
  background-image: url("../assets/mobile/image-fisheye.jpg");
}

@media (min-width: 800px) {
  section {
    padding: 0 8rem;
  }
  ul {
    grid-template-columns: 1fr 1fr 1fr 1fr;
    grid-template-rows: repeat(2, 28rem);
  }
  li {
    background-position: center center;
  }
  .deep-earth {
    background-image: url("../assets/desktop/image-deep-earth.jpg");
  }
  .night-arcade {
    background-image: url("../assets/desktop/image-night-arcade.jpg");
  }
  .soccer-team {
    background-image: url("../assets/desktop/image-soccer-team.jpg");
  }
  .deep-earth {
    background-image: url("../assets/desktop/image-deep-earth.jpg");
  }
  .the-grid {
    background-image: url("../assets/desktop/image-grid.jpg");
  }
  .from-up {
    background-image: url("../assets/desktop/image-from-above.jpg");
  }
  .pocket-borealis {
    background-image: url("../assets/desktop/image-pocket-borealis.jpg");
  }
  .the-curiosity {
    background-image: url("../assets/desktop/image-curiosity.jpg");
  }
  .make-fisheye {
    background-image: url("../assets/desktop/image-fisheye.jpg");
  }
}
</style>
