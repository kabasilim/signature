<template>
  <div id="app">
    <header>
      <h1>Signature Cardio & Fitness Center</h1>
    </header>

    <main>
      <section class="classes">
        <h2>Our Fitness Classes</h2>
        <div v-for="cls in classes" :key="cls.id">
          <ClassCard :class-data="cls" />
        </div>
      </section>

      <section class="trainers">
        <h2>Meet Our Trainers</h2>
        <div v-for="trainer in trainers" :key="trainer.id">
          <TrainerCard :trainer-data="trainer" />
        </div>
      </section>

      <section class="contact">
        <h2>Contact Us</h2>
        <ContactForm />
      </section>
    </main>

    <footer>
      <p>&copy; {{ new Date().getFullYear() }} Signature Cardio & Fitness Center</p>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      classes: [
        /* Add your class data here 
          { id: 1, name: 'Zumba', description: 'High-energy dance fitness class...', ... },
          ... 
        */
      ],
      trainers: [
        /* Add your trainer data here 
          { id: 1, name: 'John Doe', bio: 'Certified personal trainer...', ... },
          ... 
        */
      ],
    };
  },
};
</script>

<style scoped>
/* Add your styles here */
</style>
