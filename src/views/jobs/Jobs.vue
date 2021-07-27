<template>
  <div class="jobs">
      <h1>Jobs</h1>
      <div v-for="job in jobs" :key="job.id">
          <router-link :to="{name:'JobDetails', params: { id: job.id}}">
              <h3>{{job.title}}</h3>
          </router-link>
      </div>
  </div>
</template>

<script>
export default {
    name:'Jobs',
    data () {
        return {
            jobs: [
                {
                    title: "Ninja Web Developer",
                    id: 1,
                    details: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dolorem, dolores!"
                },
                {
                    title: "Ninja Ux Designer",
                    id : 2,
                    details: "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Perspiciatis, similique!"
                },
                {
                    title: "Ninja Vue Developer",
                    id : 3,
                    details: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Aperiam, vitae."
                }
            ]
        }
    }
}
</script>

<style>
.jobs h3{
    background-color: #f4f4f4;
    padding: 20px;
    border-radius: 10px;
    margin : 10px auto;
    max-width: 600px;
    cursor: pointer;
    color: #444;
}

.jobs h3:hover{
    background-color:#ddd;
}

.jobs a {
    text-decoration: none;
}

</style>