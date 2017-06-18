<template lang="html">
  <div class="">
    <div class="flex-container">
      <div class="grid" @click="move" id="1">
        <img v-if="count % 2 !== 0" src="../assets/x-mark.png" class="move">
        <img v-if="count % 2 === 0 && count > 0" src="../assets/o-mark.png" class="move">
      </div>
      <div class="grid" @click="move" id="2">
        <img v-if="count % 2 !== 0" src="../assets/x-mark.png" class="move">
        <img v-if="count % 2 === 0 && count > 0" src="../assets/o-mark.png" class="move">
      </div>
      <div class="grid" @click="move" id="3">
        <img v-if="count % 2 !== 0" src="../assets/x-mark.png" class="move">
        <img v-if="count % 2 === 0 && count > 0" src="../assets/o-mark.png" class="move">
      </div>
      <div class="grid" @click="move" id="4">
        <img v-if="count % 2 !== 0" src="../assets/x-mark.png" class="move">
        <img v-if="count % 2 === 0 && count > 0" src="../assets/o-mark.png" class="move">
      </div>
      <div class="grid" @click="move" id="5">
        <img v-if="count % 2 !== 0" src="../assets/x-mark.png" class="move">
        <img v-if="count % 2 === 0 && count > 0" src="../assets/o-mark.png" class="move">
      </div>
      <div class="grid" @click="move" id="6">
        <img v-if="count % 2 !== 0" src="../assets/x-mark.png" class="move">
        <img v-if="count % 2 === 0 && count > 0" src="../assets/o-mark.png" class="move">
      </div>
      <div class="grid" @click="move" id="7">
        <img v-if="count % 2 !== 0" src="../assets/x-mark.png" class="move">
        <img v-if="count % 2 === 0 && count > 0" src="../assets/o-mark.png" class="move">
      </div>
      <div class="grid" @click="move" id="8">
        <img v-if="count % 2 !== 0" src="../assets/x-mark.png" class="move">
        <img v-if="count % 2 === 0 && count > 0" src="../assets/o-mark.png" class="move">
      </div>
      <div class="grid" @click="move" id="9">
        <img v-if="count % 2 !== 0" src="../assets/x-mark.png" class="move">
        <img v-if="count % 2 === 0 && count > 0" src="../assets/o-mark.png" class="move">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      xsrc: '/assets/x-mark.png',
      osrc: '/assets/o-mark.png',
      count: 0
    }
  },
  methods: {
    move () {
      this.count++
    }
  }
}
</script>

<style lang="css">
.flex-container {
  display: flex;
  flex-wrap: wrap;
  width: 660px;
  margin: auto;
}

.grid {
  box-sizing: border-box;
  width: 200px;
  border: 1px solid grey;
  border-radius: 20px;
  height: 200px;
  margin: 10px;
  cursor: pointer;

  display: flex;
  justify-content: center;
  align-items: center;
}

.move {
  width: 90%;
  height: 90%;
}
</style>
