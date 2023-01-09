<template>
  <LearningResources />
</template>
<script>
import LearningResources from '@/components/learning-resource/LearningResources.vue';
export default {
  components: {
    LearningResources,
  },
  data() {
    return {
      storedMessages: [
        {
          id: 'Official-guide',
          title: 'Official Guide',
          description: 'The official Vue.js documentation',
          link: 'https://vuejs.org',
        },
        {
          id: 'google',
          title: 'Google',
          description: 'Learn to google',
          link: 'https://www.google.com',
        },
      ],
    };
  },
};
</script>
