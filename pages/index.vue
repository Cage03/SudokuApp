<script setup>
  const page = ref("HomeScreen")

</script>


<template>
  <div>
    <component :test="test" :is="page" />
  </div>
</template>



<script>
export default {
  name: 'IndexPage',
  data() {
    return {
       page:"HomeScreen",
      test: "page"
    }
  },
}
</script>
