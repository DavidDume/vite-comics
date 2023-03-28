<script>

    export default {
        name: "Jumbotron",
        props: {
            image: String,
            title: String
        }
    }

</script>

<template>
    <main>
        <div class="card">
            <img :src="image" :alt="title">
            <h3>{{ title }}</h3>
        </div>
    </main>
</template>

<style scoped lang="scss">


main {
    color: white;
    padding: 40px 0;
}

.card {
    & img {
        width: 100%;
    }
}

</style>