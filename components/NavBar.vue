<template>
  <div>
    <div class="flex justify-between px-4 py-4">
      <div class="flex space-x-7">
        <div>
          <!-- Website Logo -->
          <a href="#" class="flex items-center">
            <img class="h-16" src="~/../assets/images/logo.png" />
          </a>
        </div>
        <!-- Primary Navbar items -->
        <div class="hidden md:flex items-center">
          <a class="nav-item">About</a>
          <a class="nav-item">Roadmap</a>
          <a class="nav-item">Team</a>
          <a class="nav-item">Provenance</a>
        </div>
      </div>
      <!-- Secondary Navbar items -->
      <div class="hidden md:flex items-center">
        <a href="something" class="button"
          ><i class="fab fa-ethereum"></i> Connect Wallet</a
        >
      </div>

      <!-- Mobile menu button -->
      <div class="md:hidden flex items-center">
        <button @click="toggleMenu">
          <i class="fas fa-bars fa-2x"></i>
        </button>
      </div>
    </div>

    <!-- mobile menu -->
    <div :class="{ hidden: !menu.isActive }">
      <div class="md:hidden flex flex-col ml-4">
        <a class="nav-item">About</a>
        <a class="nav-item">Roadmap</a>
        <a class="nav-item">Team</a>
        <a class="nav-item">Provenance</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      menu: {
        isActive: false,
      },
    };
  },
  methods: {
    toggleMenu() {
      this.menu.isActive = !this.menu.isActive;
    },
  },
};
</script>

<style>
.nav {
  display: flex;
  align-items: center;
  padding: 1rem 1rem;
}

.nav-menu {
  margin-left: 4rem;
}

.nav-item {
  font: 30px HighSchool;
  text-transform: uppercase;
  color: white;
  margin-right: 2rem;
}

.nav-logo {
  width: auto;
  height: 8rem;
}

a.button {
  display: inline-block;
  padding: 0.3em 0.6em;
  margin-left: auto;
  border-radius: 2em;
  box-sizing: border-box;
  text-decoration: none;
  font: 24px HighSchool;
  color: #ffffff;
  text-align: center;
  border: solid white 3px;
  transition: all 0.2s;
}

a.button:hover {
  background-color: white;
  color: #1d1d1d;
}

@media (max-width: 950px) {
  a.button {
    font: 18px HighSchool;
  }
  .nav-item {
    font-size: 22px;
  }
}
</style>
