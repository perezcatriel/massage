<template>
  <header class="header">
    <div class="logo">
      <img src="../assets/jeri massage Logo.png" alt="Jeri Massage" />
    </div>
    <!-- Ícono de menú para móviles -->
    <div class="menu-icon" @click="toggleMenu">
      <span :class="menuOpen ? 'open' : ''"></span>
      <span :class="menuOpen ? 'open' : ''"></span>
      <span :class="menuOpen ? 'open' : ''"></span>
    </div>
    <nav :class="{ 'menu-open': menuOpen }">
      <ul>
        <li><a href="#services">Serviços</a></li>
        <li><a href="#about">Nós</a></li>
        <li><a href="#testimonials">Depoimentos</a></li>
        <li><a href="#contact">Contato</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "CxHeader",
  data() {
    return {
      menuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.menuOpen = !this.menuOpen;
    },
  },
};
</script>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px;
  background-color: var(--color-accent);
  position: relative;
}

.logo img {
  width: 40px;
  height: 40px;
  border-radius: 50%;
}

/* Ícono de menú hamburguesa */
.menu-icon {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  width: 30px;
  height: 25px;
  cursor: pointer;
}

.menu-icon span {
  display: block;
  width: 100%;
  height: 4px;
  background-color: var(--color-base);
  transition: transform 0.3s ease, opacity 0.3s ease;
}

/* Animación del ícono cuando está abierto */
.menu-icon span.open:nth-child(1) {
  transform: translateY(10px) rotate(45deg);
}
.menu-icon span.open:nth-child(2) {
  opacity: 0;
}
.menu-icon span.open:nth-child(3) {
  transform: translateY(-10px) rotate(-45deg);
}

/* Estilos del menú móvil cerrado */
nav {
  position: absolute;
  top: 100%;
  right: 0;
  background-color: var(--color-accent);
  width: 100%;
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.3s ease;
}

/* Cuando el menú está abierto */
nav.menu-open {
  max-height: 200px;
  z-index: 100;
}

nav ul {
  list-style: none;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;
  padding: 0;
  margin: 10px 0;
}
nav a:hover {
  color: var(--color-second);
}
nav a {
  text-decoration: none;
  color: var(--color-base);
  font-size: 21px;
  padding: 10px;
}

/* Estilos para pantallas más grandes (escritorio) */
@media (min-width: 768px) {
  .menu-icon {
    display: none;
  }

  .header {
    flex-direction: row;
  }

  nav {
    position: static;
    max-height: none;
    width: auto;
  }

  nav ul {
    flex-direction: row;
    gap: 20px;
  }

  nav a {
    font-size: 16px;
    padding: 0;
  }

  .logo img {
    width: 50px;
    height: 50px;
  }
}
</style>
