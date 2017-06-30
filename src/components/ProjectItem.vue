<template lang="html">
  <li class="project-item_element">
     <router-link :to="{ name: 'project', params: {projectId: project_id } }">{{ project_data.title }}</router-link>
  </li>
</template>

<script>
export default {
  name: 'project-item',
  props: ['project_id', 'project_data']
}
</script>

<style lang="css">
.project-item_element {
  width: 50%;
  background-color: #ccc;
}
</style>
