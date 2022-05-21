<template>
  <div>
 <Header />
  <Sudoku />
  <Footer />
  </div>
</template>



<script>
// import Sudoku from "~/components/Sudoku";
import Header from "~/globals/Header";
import Footer from "~/globals/Footer";
export default {
  name: 'IndexPage',
  components: {Footer, Header},
  data() {
    return {
      showSudoku: false
    }
  },
}
</script>
