<template>
    <StoredResources :resources="storedResources"/>
</template>

<script>
import StoredResources from './components/learning-resources/StoredResources.vue';

export default {
    components: {
        StoredResources,
    },
    data() {
        return {
            storedResources: [
                {
                    id: 'offcial-guide',
                    title: 'Offcial Guide',
                    description: 'The official Vue.js documentation',
                    link: 'https://vuejs.org'
                },
                {
                    id: 'google',
                    title: 'Google',
                    description: 'Learn to google...',
                    link: 'https://google.pt'
                }
            ],
        }
    }
}
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