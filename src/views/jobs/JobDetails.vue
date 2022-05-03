<template>
    <div>
        <h1>job details page</h1>
        <p>the job is {{ $route.params.id }}</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            id: this.$route.params.id
        }
    }
}
</script>

<style>
</style>