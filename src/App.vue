<template>
  <div>
    <TheHeader title="RememberMe" />
    <StoredResources :resources="StoredResources" />
  </div>
</template>

<script>
import StoredResources from './components/learning-resource/StoredResources.vue';
import TheHeader from './components/layouts/TheHeader.vue';
export default {
  components: {
    StoredResources,
    TheHeader,
  },
  data() {
    return {
      StoredResources: [
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

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>
