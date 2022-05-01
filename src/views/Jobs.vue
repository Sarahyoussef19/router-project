<template>

    <h1>Jobs</h1>
    <div v-for="Job in jobs" :key="job.id">
        <h1>{{ Jobs.title }} </h1>
    </div>

</template>

<script>
export default {
    data() {
        return {
            jobs: [
                { title: 'web developer', id: 1, details: 'lorem' },
                { title: 'web designer', id: 2, details: 'lorem' },
                { title: 'web3 expert', id: 3, details: 'lorem' },
                { title: 'CEO', id: 4, details: 'lorem' },
            ]
        }
    }
}
</script>

<style>
</style>