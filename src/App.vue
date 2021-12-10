npm<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  components: {
  },

  data() {
    return {
      count:0,
      messages: [
                {
                    'number' : 1,
                    'image' : 'img/1.png',
                    'content' : 'Message'
                },
                {
                    'number' : 2,
                    'image' : 'img/1.png',
                    'content' : 'Message'
                },
                {
                    'number' : 3,
                    'image' : 'img/1.png',
                    'content' : 'Message'
                },
                {
                    'number' : 4,
                    'image' : 'img/1.png',
                    'content' : 'Message'
                },
                {
                    'number' : 5,
                    'image' : 'img/1.png',
                    'content' : 'Message'
                },
                {
                    'number' : 6,
                    'image' : 'img/1.png',
                    'content' : 'Message'
                },
                {
                    'number' : 7,
                    'image' : 'img/7.png',
                    'content' : 'Message'
                },
                {
                    'number' : 8,
                    'image' : 'img/8.png',
                    'content' : 'Message'
                },
                {
                    'number' : 9,
                    'image' : 'img/9.png',
                    'content' : 'Message'
                },
                {
                    'number' : 10,
                    'image' : 'img/10.png',
                    'content' : 'Message'
                },
                {
                    'number' : 11,
                    'image' : 'img/11.png',
                    'content' : 'Message'
                },
                {
                    'number' : 12,
                    'image' : 'img/12.png',
                    'content' : 'Message'
                },
                {
                    'number' : 13,
                    'image' : 'img/13.png',
                    'content' : 'Message'
                },
                {
                    'number' : 14,
                    'image' : 'img/14.png',
                    'content' : 'Message'
                },
                {
                    'number' : 15,
                    'image' : 'img/15.png',
                    'content' : 'Message'
                },
                {
                    'number' : 16,
                    'image' : 'img/16.png',
                    'content' : 'Message'
                },
                {
                    'number' : 17,
                    'image' : 'img/17.png',
                    'content' : 'Message'
                },
                {
                    'number' : 18,
                    'image' : 'img/18.png',
                    'content' : 'Message'
                },
                {
                    'number' : 19,
                    'image' : 'img/19.png',
                    'content' : 'Message'
                },
                {
                    'number' : 20,
                    'image' : 'img/20.png',
                    'content' : 'Message'
                },
                {
                    'number' : 21,
                    'image' : 'img/21.png',
                    'content' : 'Message'
                },
                {
                    'number' : 22,
                    'image' : 'img/22.png',
                    'content' : 'Message'
                },
                {
                    'number' : 23,
                    'image' : 'img/23.png',
                    'content' : 'Message'
                },
                {
                    'number' : 24,
                    'image' : 'img/24.png',
                    'content' : 'Message'
                },
            ],
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
    <h1>Calendrier de l'avent 2019</h1>
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
