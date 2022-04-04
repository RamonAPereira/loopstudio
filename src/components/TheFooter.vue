<template>
  <footer>
    <div>
      <img src="../assets/logo.svg" alt="" />
      <ul class="links">
        <li><a href="#">About</a></li>
        <li><a href="#">Careers</a></li>
        <li><a href="#">Events</a></li>
        <li><a href="#">Products</a></li>
        <li><a href="#">Support</a></li>
      </ul>
    </div>
    <div>
      <ul class="social">
        <li>
          <a href="#"><img src="../assets/icon-facebook.svg" alt="" /></a>
        </li>
        <li>
          <a href="#"><img src="../assets/icon-twitter.svg" alt="" /></a>
        </li>
        <li>
          <a href="#"><img src="../assets/icon-pinterest.svg" alt="" /></a>
        </li>
        <li>
          <a href="#"><img src="../assets/icon-instagram.svg" alt="" /></a>
        </li>
      </ul>
      <p>&copy; 2022 Loopstudios. All rights reserved</p>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style scoped>
footer {
  background: hsl(0, 0%, 0%);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 2rem;
  padding: 4rem 0;
  margin-top: 4rem;
}
li {
  color: hsl(0, 0%, 100%);
  text-align: center;
  font-size: 15px;
}
li:hover {
  border-bottom: 1px solid hsl(0, 0%, 100%);
  transition: all 0.3s ease-in;
}

.social {
  display: flex;
  justify-content: center;
  gap: 1rem;
}
.links {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}
div {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

@media (min-width: 800px) {
  footer {
    flex-direction: row;
    justify-content: space-between;
    padding: 4rem 8rem;
  }
  .links {
    flex-direction: row;
  }
  div {
    gap: 4rem;
  }
  img {
    max-width: 15rem;
  }
}
</style>
