<template>
    <li>
        <base-card>
            <div class="col-10">
                <header>
                    <h3>{{ title }}</h3>
                </header>
                <p>{{ description }}</p>
                <nav>
                    <a :href="link">View resource</a>
                </nav>
            </div>
            <div class="col">
                <button class="btn btn-secondary">Delete</button>
            </div>
        </base-card>
    </li>
</template>

<script>
export default {
    props: ['title', 'description', 'link']
}
</script>
<style scoped>
li{
    list-style-type: none;
}
</style>