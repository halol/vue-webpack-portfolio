<template>
  <div class="hello">
    <h5>Featured Projects</h5>
    {{projects}}
    {{works}}
    <ul>
      <project-item v-for="(index, value) in projects" :project_data="index" :project_id="value" :key="index"></project-item>
    </ul>
  </div>
</template>

<script>
import ProjectItem from '@/components/ProjectItem'
import projects from '@/data.json'

const works = [
  {
    title: 'Work 1'
  }
]
export default {
  name: 'hello',
  data () {
    return {
      // msg: 'Welcome to Your Vue.js App'
      projects,
      works
    }
  },
  components: {
    'project-item': ProjectItem
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h5 {
  text-transform: uppercase;
  letter-spacing: 0.1em;
}
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}


a {
  color: #42b983;
}
</style>
