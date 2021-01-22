<template>
  <div class="Student-Detail">
    <h1>{{ Student.title }}</h1>
    <br />
    <div style="padding: 0px 0px 0px 3px; font-size: 40px">
      <b>NAME</b> {{ Student.studentName }} <br />
    </div>
    <br />
    <div>
      <img
        style="float: left; padding: 20px"
        width="250px"
        v-bind:src="Student.picture"
      />
    </div>
    <div style="padding: 0px 0px 10px 400px">
      <b>StudentId:</b> {{ Student.studentId }} <br />
      <br /><b>FirstName:</b> {{ Student.FirstName }} <br />
      <br /><b>LastName:</b> {{ Student.LastName }}<br />
      <br /><b>Weight:</b> {{ Student.weight }} <br />
      <br /><b>Height:</b> {{ Student.height }} <br />
      <br />
      <br />
    </div>
  </div>
</template>



<script>
export default {
  name: "StudentDetail",
  components: {},
  props: ["Student"],
};
</script>

<style>
.Student-Detail {
  background: rgb(fff, fff, fff);
  padding: 20px 30px 0px 400px;
  border-bottom: indigo 1px;
}
</style>