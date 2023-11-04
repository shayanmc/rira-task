<template>
  <div class="text-center">
    <button @click="Decrease" class="button">-</button>
    <span>{{number}}</span>
    <button @click="increase" class="button">+</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      number : 0
    }
  },
  methods: {
    increase () {
        this.number += 1
    },
    Decrease () {
        this.number -= 1
    }
   }
}
</script>

<style >

html,body {
  margin:0;
  padding:0;
  overflow: hidden; /* Hide scrollbar */

}
* {
  background-color: rgb(51 65 85);
}
span {
  font-size: 40px;
  color: #ffffff;
}
.text-center {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  height: 700px;
}
.button {
  background:    #f0ac46;
  border-radius: 28px;
  padding:       18px  35px;
  color:         #ffffff;
  display:       inline-block;
  font:          normal normal 33px/1 "Open Sans", sans-serif;
  text-align:    center;
  border: none; 
}

.button:hover,
.button:active {
  cursor: pointer;
  background:    #eccfa2;
}

</style>
