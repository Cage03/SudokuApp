<template>
  <div>
    {{name}}
    <div class="sudoku-container">
      <div class="sudoku-grid">
        <!--todo replaced by sudoku components-->
        <!--Contains row and block, used to generate divs from code -->
        <div class="sudoku-blocks-container">
<!--          <div class="sudoku-row"></div>-->
<!--          <div class="sudoku-block">-->
<!--            <p></p>-->
<!--          </div>-->
<!--          todo style the components -->
          <Row   v-for="nr in 9" key="int" :number="nr"/>
        </div>
      </div>
    </div>

    <div class="draw-controls-container">
      <!--Pencil can be clicked to make notes within the sudoku grid -->
      <label id="pencil-label"></label>
      <div class="pencil-container"></div>
      <!--Pen can be clicked to make submit answers within the sudoku grid -->
      <label id="pen-label"></label>
      <div class="pen-container"></div>

      <!--Numbers can be clicked to select a input number -->
      <div class="number-grid">
        <div class="number-block">1</div>
        <div class="number-block">2</div>
        <div class="number-block">3</div>
        <div class="number-block">4</div>
        <div class="number-block">5</div>
        <div class="number-block">6</div>
        <div class="number-block">7</div>
        <div class="number-block">8</div>
        <div class="number-block">9</div>
      </div>
    </div>

    <div class="mistakes-container">
      <p>Mistakes: 0/3</p>
    </div>

    <!--Onclick should generate a different sudoku than the previous one -->
    <button class="new-sudoku">Generate new sudoku</button>

  </div>
</template>

<script>


import Row from "./Sudoku/Row";
export default {
  name: "Sudoku",
  components: {Row},
  data: () => ({
    name: "Sudoku",
  }),

}

function generateGrid(){
  $()
}

</script>

<style scoped>

</style>
