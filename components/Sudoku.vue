<template>
  <div>
    {{name}}
    <div class="sudoku-container">
      <div class="sudoku-grid">
        <!--Contains row and block, used to generate divs from code -->
        <div class="sudoku-blocks-container" style="visibility:hidden;">
          <div class="sudoku-row"></div>
          <div class="sudoku-block">
            <p></p>
          </div>
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
export default {
  name: "Sudoku",
  data: () => ({
    name: "Sudoku",
  }),

}
</script>

<style scoped>

</style>
