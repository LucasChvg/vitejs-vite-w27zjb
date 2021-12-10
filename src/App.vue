npm<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  components: {
  },

  data() {
    return {
      count:0,

    };
  },

  methods: {
    increment(){
      this.count++;
    },
    reset(){
      this.count = 0;
    },
  },
});

</script>

<template>
  <h1>Weihnachtskalender 2021</h1>
  <div class="jumbotron text-center" style="margin-bottom:0; background-color: darkred; color: white;">
    <h1>Calendrier de l'avent 2021</h1>
    <p>Hoo Hoo Hoooooo ! Voici quelques indices pour ton calendrier de l'avent :p</p>
  </div>
  <div class="calendar">
    {{count}}
  </div>
  <div class="container-fluid" style="margin-top:30px" id="app">
    <div class="row">
        <div class="col-lg-2 col-md-3 col-sm-6 col-xs-12" v-for="message in messages">
            <p>hello</p> 
        </div>
    </div>
  </div>
  <button @click="increment">Click Me</button>
  <button @click="reset">Reset</button>

</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Mountains+of+Christmas:wght@700&display=swap');

#app {
  font-family: 'Mountains of Christmas', cursive;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 10px;
}

/* This creates a 6x4 grid with 140px wide squares */
.calendar {
  display: grid;
  grid-template-columns: repeat(6, 140px);
  grid-template-rows: repeat(4, 140px);
  gap: 20px;
}
</style>
