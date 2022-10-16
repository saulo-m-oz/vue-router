<template>
  <h1>Jobs Details Page!!</h1>
  <p>The Job ID is: {{id}}</p>
  <p>Job Details: {{ details }}</p>
</template>

<script>
export default {
    props: ["id", "details"],
}
</script>

<style>

</style>