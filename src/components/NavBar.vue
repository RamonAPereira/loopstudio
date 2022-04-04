<template>
  <header>
    <nav>
      <img src="../assets/logo.svg" alt="" />
      <a href="#" @click.prevent="showMenu"
        ><img class="hamburger" src="../assets/icon-hamburger.svg" alt=""
      /></a>
      <ul>
        <li><a href="#">About</a></li>
        <li><a href="#">Careers</a></li>
        <li><a href="#">Events</a></li>
        <li><a href="#">Products</a></li>
        <li><a href="#">Support</a></li>
      </ul>
    </nav>
  </header>
  <div
    class="nav-menu animate__animated animate__slideInRight"
    v-if="menuVisibility"
  >
    <ul class="menu-close">
      <li><img src="../assets/logo.svg" alt="" /></li>
      <li>
        <a href="#" @click.prevent="showMenu"
          ><img class="hamburger" src="../assets/icon-close.svg" alt=""
        /></a>
      </li>
    </ul>
    <ul class="mobile-menu">
      <li><a href="#">About</a></li>
      <li><a href="#">Careers</a></li>
      <li><a href="#">Events</a></li>
      <li><a href="#">Products</a></li>
      <li><a href="#">Support</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  data: () => ({
    menuVisibility: false,
  }),
  methods: {
    showMenu() {
      this.menuVisibility = !this.menuVisibility;
    },
  },
};
</script>

<style scoped>
header {
  position: sticky;
  top: 0;
  left: 0;
  right: 0;
  background: #000;
  z-index: 15;
}
nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 2rem;
}

a {
  color: hsl(0, 0%, 100%);
}
li:hover {
  border-bottom: 1px solid hsl(0, 0%, 100%);
  transition: all 0.3s ease-in;
}

.nav-menu {
  position: fixed;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  gap: 4rem;
  padding-top: 4rem;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background: black;
  z-index: 20;
}

@media (min-width: 800px) {
  nav {
    padding: 2rem 8rem;
  }
  .hamburger {
    display: none;
  }
}
ul {
  display: flex;
  gap: 1rem;
}
@media (max-width: 801px) {
  ul {
    display: none;
  }
  .mobile-menu {
    display: flex;
    flex-direction: column;
    align-content: center;
    justify-content: center;
    font-size: 2.5rem;
  }
  .menu-close {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 0rem 0;
    gap: 4rem;
  }
}
</style>
