<template>
  <div class="pagination-container">
    <div class="pagination-controls">
      <button class="page-left">❮ &nbsp;</button>
      <button>1</button>
      <button>2</button>
      <button>...</button>
      <button>9</button>
      <button>10</button>
      <button class="page-right">❯ &nbsp;</button>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.pagination-container {

  width: 100%;
}
.pagination-controls {
  display: flex;
  justify-content: flex-end;
  /* background: red; */
  width: 95%;
}
.pagination-controls button {
  background: #ffffff;
  border: 1px solid #dfe3e8;
  box-sizing: border-box;
  border-radius: 30px;
  font-size: 14px;
  line-height: 20px;
  text-align: center;
  color: #212b36;
  margin-right: 8px;
  padding: 1px 4px;
}
.prev,
.next {
  color: #c4cdd5;
}
.prev {
  background: #919eab;
}
.one {
  border: 1px solid #dfe3e8;
}
</style>
