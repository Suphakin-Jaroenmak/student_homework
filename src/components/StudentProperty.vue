<template>
  <div>
    <div v-bind:key="Student.StudentId" v-for="Student in StudentIndex">
      <StudentDetail v-bind:Student="Student" />
    </div>
  </div>
</template>



<script>
//import StudentDetail
import StudentDetail from "./StudentDetail.vue";
export default {
  name: "StudentProperty",
  components: {
    StudentDetail,
  },
  props: ["StudentIndex"],
};
</script>

<style>
</style>