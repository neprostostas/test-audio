<template>
  <div class="CustomFooter">
    <footer class="footerWrapper">
      <h3>Test 2</h3>
    </footer>
  </div>
</template>

<script>

export default {
  name: 'CustomFooter',

  setup() {

    return { }
  }
}
</script>

<style scoped>

.CustomFooter {
  background: #f3f3f3;
}

.footerWrapper {
  z-index: 999;
  max-width: 1200px;
  margin: 0 auto;
  background: #f3f3f3;
  padding: 20px;
  display: grid;
  gap: 40px;
}

.footerWrapper h3 {
  color: #2d67ab;
}

</style>
