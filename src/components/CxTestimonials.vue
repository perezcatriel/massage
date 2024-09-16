<template>
  <section id="testimonials" class="testimonials">
    <h2>Depoimentos</h2>
    <div class="testimonial">
      <p>"A melhor massagem que já recebi. Estarei de volta em breve."</p>
      <p>- Cliente Satisfeito</p>
    </div>
  </section>
</template>

<script>
export default {
  name: "CxTestimonials",
};
</script>

<style scoped>
.testimonials {
  padding: 50px;
  background-color: var(--color-base);
  text-align: center;
  font-size: 1rem;
}
p {
  color: var(--color-accent);
}
</style>
