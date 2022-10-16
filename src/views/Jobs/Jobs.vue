<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.id" class="job">
    <router-link :to="{name: 'JobDetails', params: {id: job.id}}"> <h2>{{job.title}}</h2> </router-link>
  </div>
</template>

<script>
export default {
    data(){
        return{
            jobs: [
                {title: "Front End Jr", id: 1, details: "React needed"},
                {title: "Front End Jr", id: 2, details: "VueJS needed"},
                {title: "Back End Jr", id: 3, details: "NodeJS with Express needed"},
                {title: "Front End Jr", id: 4, details: "DJANGO needed"},
            ]
        }
    }
}
</script>

<style>
  .job h2{
    background: #f4f4f4;
    padding: 20px;
    border-radius: 10px;
    margin: 10px auto;
    max-width: 600px;
    cursor: pointer;
    color: #444;
  }
  .job h2:hover{
    background: #ddd;
  }
  .job a{
    text-decoration: none;
  }
</style>