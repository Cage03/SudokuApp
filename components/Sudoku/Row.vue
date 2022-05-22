<template>
<!--  todo replace inline style-->
  <div class="sudoku-row" style="display: flex">
    <!--  spawns 9 blocks passing row and collumn  -->
    <SudokuBlock v-for="nr in 9" key="int" :number="nr" :name="getRowName(number)"/>
  </div>
</template>

<script>
import Sudoku from "../Sudoku";

export default {
  name: "Row",
  components: {Sudoku},
  props: {
    number: {
      type: Number,
      required: true
    }
  },
  methods: {
    getRowName: function (nr) {
      let nameArray = ["A", "B", "C", "D", "E", "F", "G", "H", "I"];
      return nameArray[nr - 1];
    }
  }
}
</script>

<style scoped>

</style>
