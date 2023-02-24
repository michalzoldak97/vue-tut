<template>
    <the-header></the-header>
    <stored-resources :resources="storedResources"></stored-resources>
</template>

<script>
import TheHeader from './components/layouts/TheHeader.vue';
import StoredResources from './components/learning-resources/StoredResources.vue';

export default {
    components: {
        StoredResources,
        TheHeader
    },
    data() {
        return {
            storedResources: [
                {
                    id: 'test-one',
                    title: 'Test One',
                    description: 'This is the Test One',
                    link: 'https://vuejs.org',
                },
                {
                    id: 'test-two',
                    title: 'Test Two',
                    description: 'This is the Test Two',
                    link: 'https://google.com',
                },
            ],
        };
    },
};
</script>
