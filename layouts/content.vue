<template>
  <div class="layout-container">
    <div class="header-container">
      <householdheader />
    </div>
    <!-- <div class="container"> -->
      <div class="sidebar">
        <sidenav />
      </div>
      <div class="main-section">
        <Nuxt />
      </div>
    <!-- </div> -->
  </div>
</template>

<script>
export default {
  name: 'content',
}
</script>

<style>
html {
  word-spacing: 1px;
  line-height: 18px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background-color: #f3f6f8;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.layout-container {
min-width: 100%;
}

.container {
  display: flex;
  padding-top: 90px;
  /* border: 1px solid red; */
  margin-left: 110px;
}

.main-section {
  margin: 20px 0 0 245px;
  /* border: 1px solid; */
  background-color: #F3F6F8;
}
.sidebar{
  padding-top: 74px;
}
</style>
</style>