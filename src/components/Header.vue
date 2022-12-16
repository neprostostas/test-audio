<template>
  <div class="CustomHeader">
    <header>
      <div class="headerWrapperColor">
        <div class="headerWrapper">
          <h2>Audio Library</h2>
        </div>
      </div>
    </header>
  </div>
</template>

<script>

export default {
  name: 'CustomHeader',

  setup() {

    return { }
  }
}
</script>

<style scoped>

.headerWrapperColor {
  background: #f3f3f3;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 999;
}

.headerWrapper {
  z-index: 999;
  max-width: 1200px;
  margin: 0 auto;
  background: #f3f3f3;
  padding: 20px;
  display: grid;
  gap: 40px;
}

.headerWrapper h2 {
  color: #47c5c5;
}

</style>