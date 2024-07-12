te>
  <div class="class-card">
    <h3>{{ classData.name }}</h3>
    <p>{{ classData.description }}</p>
    <button>Learn More</button>
  </div>
</template>

<script>
export default {
  props: {
    classData: Object,
  },
};
</script>

<style scoped>
.class-card {
  /* Add your styles here */
}
</style>

