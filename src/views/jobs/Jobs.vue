<template>

    <h1>Jobs</h1>
    <div v-for="Job in Jobs" :key="Job.id">
        <router-link :to="{ name: 'JobDetails', params: { id: Job.id } }">
            <h2>{{ Job.title }}</h2>
        </router-link>
    </div>

</template>

<script>
export default {
    data() {
        return {
            Jobs: [
                { title: 'web developer', id: 1, details: 'lorem' },
                { title: 'web designer', id: 2, details: 'lorem' },
                { title: 'web3 expert', id: 3, details: 'lorem' },
            ]
        }
    }
}
</script>

<style>
a {
    text-decoration: none;
}

h2 {
    background-color: antiquewhite;
    color: rgb(10, 10, 145);
    padding: 15px;
    border-radius: 20px;
    width: 500px;
    margin: 10px auto;
    cursor: pointer;

}

h2:hover {
    background-color: black;
    color: aliceblue;
}
</style>