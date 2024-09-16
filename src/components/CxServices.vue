<template>
  <section id="services" class="services">
    <h2>Nuestros Servicios</h2>
    <div class="service-list">
      <div class="service">
        <img src="../assets/jeri massage Logo.png" alt="Masaje Relajante" />
        <h3>Massagem Sueca</h3>
        <p>Desconecte-se e desfrute de um momento de paz.</p>
        <h3>R$ 150</h3>
      </div>
      <div class="service">
        <img src="../assets/jeri massage Logo.png" alt="Masaje Terapéutico" />
        <h3>Massagem Tailandesa</h3>
        <p>Alivie a tensão e melhore o seu bem-estar físico.</p>
        <h3>R$180</h3>
      </div>
      <div class="service">
        <img src="../assets/jeri massage Logo.png" alt="Masaje Terapéutico" />
        <h3>Massagem Ayurvédica</h3>
        <p>
          Prática milenar, amassamento e óleos
          para equilibrar os doshas.
        </p>
        <h3>R$200</h3>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "CxServices",
};
</script>

<style scoped>
.services {
  padding: 50px;
  background-color: var(--color-base);
  text-align: center;
}

.services h2 {
  color: var(--color-accent);
  margin-bottom: 30px;
  font-size: 2.5rem;
}

.service-list {
  display: flex;
  flex-wrap: wrap; /* Asegura que los elementos se ajusten en pantallas más pequeñas */
  gap: 20px;
  justify-content: center;
}

.service {
  border: 2px solid var(--color-second);
  border-radius: 10px;
  padding: 20px;
  background-color: #fff;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  width: 100%;
  max-width: 300px;
}

.service img {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  margin-bottom: 15px;
  transition: transform 0.3s ease;
}

.service h3 {
  color: var(--color-accent);
  margin-bottom: 10px;
}

.service p {
  color: var(--color-second);
}

.service:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
}

.service img:hover {
  transform: scale(1.1);
}

/* Estilos para pantallas más pequeñas */
@media (max-width: 600px) {
  .service-list {
    flex-direction: column;
    align-items: center;
  }
}
</style>
