<template lang="html">
  <div class="">
    <router-link :to="{path: '/'}">Back</router-link>
    <h1>{{ projectData.title }}</h1>
    <img src="//lorempixel.com/g/400/200" alt="" class="image">
    <p class="project-content-item__description" v-if="projectData.description">{{ projectData.description }}</p>
  </div>

</template>

<script>
import projects from '@/data.json'
export default {
  name: 'project',
  data () {
    return {
      projectData: projects[this.$route.params.projectId]
    }
  }
}
</script>

<style lang="css">
.image {
  width: 100%;
}
</style>
