te>
  <div class="trainer-card">
    <img :src="`images/${trainerData.id}.jpg`" alt="Trainer Image">
    <h3>{{ trainerData.name }}</h3>
    <p>{{ trainerData.bio }}</p>
  </div>
</template>

<script>
export default {
  props: {
    trainerData: Object,
  },
};
</script>

<style scoped>
.trainer-card {
  /* Add your styles here */
}
</style>

