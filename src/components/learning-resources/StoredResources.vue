<template>
    <div class="container-sm">
        <ul>
            <learning-resource v-for="res in resources" 
                :key="res.id"  
                :title="res.title" 
                :description="res.description"
                :link="res.link"
                ></learning-resource>
        </ul>
    </div>
</template>

<script>
import LearningResource from './LearningResource.vue';

export default {
    components: {
        LearningResource
    },
    props: ['resources']
};
</script>