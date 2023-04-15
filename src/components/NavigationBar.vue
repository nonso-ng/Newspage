<template>
  <div class="navbar">
    <img src="../assets/logo.svg" class="logo" />

    <ul class="desktop">
      <li>Home</li>
      <li>New</li>
      <li>Popular</li>
      <li>Trending</li>
      <li>Categories</li>
    </ul>

    <img
      src="../assets/icon-menu.svg"
      class="mobile-menu"
      @click="handleMenu"
    />

    <div class="mobile-list" v-show="menu">
      <ul class="mobile">
        <img
          class="mob_menu_close"
          src="../assets/icon-menu-close.svg"
          style="color: black; font-size: 2rem"
          @click="handleMenu"
        />
        <li>Home</li>
        <li>New</li>
        <li>Popular</li>
        <li>Trending</li>
        <li>Categories</li>
      </ul>
    </div>
  </div>
  <div class="overlay" v-show="menu"></div>
</template>

<style scoped>
.navbar {
  background-color: white;
  display: flex;
  justify-content: space-between;
  height: 15vh;
  align-items: center;
  color: grey;

  /* font-family:'Inter', sans-serif ; */
}
.navbar .logo {
  width: 6%;
  height: 35%;
}

.navbar ul {
  display: flex;
  list-style: none;
  margin-right: 15%;
}

.navbar ul li {
  font-family: "Inter", sans-serif;
  font-size: small;
  font-weight: 600;
  justify-content: space-between;
  margin-left: 15%;
}

.navbar ul li:hover {
  color: hsl(5, 85%, 63%);
}

.navbar .mobile-menu {
  display: none;
}
.navbar .mobile-list {
  display: none;
}

@media (max-width: 800px) {
  .overlay {
    position: absolute;
    top: 0%;
    left: 0%;
    width: 100%;
    height: 285vh;
    background-color: rgba(0, 0, 0, 0.6);
    z-index: 5;
  }
  .navbar {
    height: 10vh;
    background-color: white;
  }
  .navbar .logo {
    margin-left: 3%;
    width: 9%;
  }

  .desktop li {
    display: none;
  }
  .navbar .mobile-menu {
    display: flex;
    margin-right: 3%;
    height: 30%;
  }

  .navbar .mobile-list {
    display: flex;
    flex-direction: column;
    background-color: white;
    position: absolute;
    min-height: 191vh;
    width: 70%;
    z-index: 10;
    right: 0;
    justify-content: center;
    color: black;
  }

  .mob_menu_close {
    position: absolute;
    right: 10%;
    top: 50%;
  }

  .mobile {
    display: flex;

    width: 10%;
    height: 80%;

    flex-direction: column;
    gap: 3rem;
    justify-content: center;
    margin-top: 35rem;
  }
}
</style>

<script>
export default {
  data() {
    return {
      menu: false,
    };
  },
  methods: {
    handleMenu() {
      this.menu = !this.menu;
    },
  },
};
</script>
