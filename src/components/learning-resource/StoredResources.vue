<template>
  <ul>
    <LearningResources
      v-for="res in resources"
      :key="res.id"
      :id="res.id"
      :title="res.title"
      :description="res.description"
      :link="res.link"
    />
  </ul>
</template>
<script>
import LearningResources from './LearningResources.vue';
export default {
  inject: ['resources'],
  components: {
    LearningResources,
  },
};
</script>
<style scoped>
ul {
  list-style: none;
  margin: 0;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}
</style>
