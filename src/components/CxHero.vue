<template>
  <section class="hero">
    <div class="hero-overlay">
      <h1>Relaxe e revitalize-se na Jeri Massage</h1>
      <p>
        As melhores massagens de Jericoacoara, pensadas para o seu bem-estar.
      </p>
    </div>
  </section>
</template>

<script>
export default {
  name: "CxHero",
};
</script>

<style scoped>
.hero {
  position: relative;
  background-image: url("../assets/masaje.jpg");
  background-size: cover;
  background-position: center;
  height: 80vh;
  display: flex;
  justify-content: center;
  align-items: center;
  color: var(--color-base);
  text-align: center;
}

.hero-overlay {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(0, 0, 0, 0.5); /* Filtro negro translúcido */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 20px;
}

h1 {
  font-size: 2.5rem;
  margin-bottom: 10px;
  color: var(--color-accent);
  text-shadow: 1px 1px 1px var(--color-base);
}

p {
  font-size: 1.2rem;
  max-width: 600px;
  text-shadow: 1px 1px 1px var(--color-second);
}

/* Estilos para pantallas más grandes */
@media (min-width: 768px) {
  h1 {
    font-size: 3rem;
  }

  p {
    font-size: 1.5rem;
  }
}
</style>
