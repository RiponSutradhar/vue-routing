<template>
  <div class="jobdetails">
      <h1>Job Details</h1>
      <p>The job id is {{id}}</p>
  </div>
</template>

<script>
export default {
    props:['id'],
    name: "JobDetials",
    data () {
        return {
            // id : this.$route.params.id,
        }
    }

}
</script>

<style>

</style>