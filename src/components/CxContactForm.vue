<template>
  <section id="contact" class="contact">
    <h2>Contate-nos</h2>
    <form>
      <input type="text" placeholder="Nome" />
      <input type="email" placeholder="E-mail" />
      <textarea placeholder="Mensagem"></textarea>
      <button type="submit">Enviar</button>
    </form>
    <div class="footer-note">
      Criado por <a href="https://datacraft.vercel.app" target="_blank">DataCraft</a>
    </div>
    <a href="https://wa.me/5588999496039" class="whatsapp-icon" target="_blank" aria-label="WhatsApp">
      <i class="fab fa-whatsapp"></i>
    </a>
  </section>
</template>

<script>
export default {
  name: 'ContactForm',
};
</script>

<style scoped>
.contact {
  padding: 50px;
  background-color: var(--color-accent);
  width: 80vw;
  margin: auto;
  border-radius: 20px 20px 0 0;
  position: relative;
}

h2 {
  color: var(--color-second);
}

form {
  display: flex;
  flex-direction: column;
  gap: 15px;
}

button {
  background-color: var(--color-second);
  color: var(--color-base);
  border-radius: 10px;
  padding: 10px;
  border: none;
  cursor: pointer;
  font-size: 16px;
}

.footer-note {
  margin-top:  80px;
  text-align: center;
  color: var(--color-base);
}

.footer-note a {
  color: var(--color-base);
  text-decoration: none;
  font-weight: bold;
}

.footer-note a:hover {
  color: var(--color-second);
}

/* Estilos para el ícono de WhatsApp */
.whatsapp-icon {
  position: fixed;
  bottom: 20px;
  right: 20px;
  background-color: var(--color-accent);
  color: var(--color-base);
  border-radius: 50%;
  padding: 15px 16px;
  box-shadow: 0px 0px 10px var(--color-second);
  font-size: 24px;
  text-align: center;
}

.whatsapp-icon:hover {
  background-color: var(--color-second);
  color: var(--color-accent)
}

/* Asegúrate de que Font Awesome esté disponible */
@import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css');
</style>
