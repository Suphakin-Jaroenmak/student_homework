<template>
  <div id="app">
    <div class="Student-Front">
      <center>
        <h1>Information Me & Friends</h1>
      </center>
    </div>

    <StudentProperty v-bind:StudentIndex="StudentProperty" />
  </div>
</template>

<script>
import StudentProperty from "./components/StudentProperty.vue";

export default {
  name: "App",
  components: {
    StudentProperty,
  },
  data() {
    return {
      StudentProperty: [
        {
          studentName: "YUI",
          studentId: "614234007",
          FirstName: "Suphakin",
          LastName: "Jaroenmak",
          weight: 60,
          height: 163,
          picture:
            "https://github.com/Suphakin-Jaroenmak/Pixture/blob/main/Yui-1.png?raw=true",
        },
        {
          studentName: "KIK",
          studentId: "614234006",
          FirstName: "Sineenad",
          LastName: "Songsen",
          weight: 55,
          height: 162,
          picture:
            "https://github.com/Suphakin-Jaroenmak/Pixture/blob/main/kik.png?raw=true",
        },
        {
          studentName: "PRA",
          studentId: "614234022",
          FirstName: "Supansa",
          LastName: "Rodmin",
          weight: 54,
          height: 161,
          picture:
            "https://github.com/Suphakin-Jaroenmak/Pixture/blob/main/pha.png?raw=true",
        },
        {
          studentName: "KAH",
          studentId: "614234014",
          FirstName: "Nur-ateekah",
          LastName: "Salaeh",
          weight: 65,
          height: 159,
          picture:
            "https://github.com/Suphakin-Jaroenmak/Pixture/blob/main/ka.png?raw=true",
        },
        {
          studentName: "PARI",
          studentId: "614234015",
          FirstName: "Praiyapat",
          LastName: "Chaornrit",
          weight: 55,
          height: 165,
          picture:
            "https://github.com/Suphakin-Jaroenmak/Pixture/blob/main/pari.png?raw=true",
        },
      ],
    };
  },
};
</script>

<style>
#app {
  font-family: "Sedgwick Ave Display", cursive;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #586674;
  margin-top: 20px;
  font-size: 20px;
  padding: 20px 0px 0px 100px;

  background: rgb(0, 0, 0);
}

.Student-Front {
  font-size: 50px;
}
</style>