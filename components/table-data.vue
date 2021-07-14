<template>
  <div class="container">
    <table>
      <thead>
        <tr class="table-data">
          <th>User ID</th>
          <th>Registration Date</th>
          <th>Full Name</th>
          <th>Email Address</th>
          <th>User Type</th>
        </tr>
      </thead>

      <tr class="data">
        <td>1234567890</td>
        <td>23.04.2020</td>
        <td>Abdul Ifeoma</td>
        <td>amaranth@outlook.com</td>
        <td class="customer">Customer</td>
      </tr>

      <tr>
        <td>#ND1283</td>
        <td>23.04.2020</td>
        <td>Abdul Ifeoma</td>
        <td>amaranth@outlook.com</td>
        <td class="customer">Customer</td>
      </tr>

      <tr>
        <td>#ND1283</td>
        <td>23.04.2020</td>
        <td>Abdul Ifeoma</td>
        <td>amaranth@outlook.com</td>
        <td class="customer">Customer</td>
      </tr>

      <tr>
        <td>#ND1283</td>
        <td>23.04.2020</td>
        <td>Abdul Ifeoma</td>
        <td>amaranth@outlook.com</td>
        <td class="customer">Customer</td>
      </tr>

      <tr>
        <td>#ND1283</td>
        <td>23.04.2020</td>
        <td>Abdul Ifeoma</td>
        <td>amaranth@outlook.com</td>
        <td class="customer">Customer</td>
      </tr>
      <tr>
        <td>#ND1283</td>
        <td>23.04.2020</td>
        <td>Abdul Ifeoma</td>
        <td>amaranth@outlook.com</td>
        <td class="customer">Customer</td>
      </tr>
      <tr>
        <td>#ND1283</td>
        <td>23.04.2020</td>
        <td>Abdul Ifeoma</td>
        <td>amaranth@outlook.com</td>
        <td class="customer">Customer</td>
      </tr>

      <div class="pagination-container">
        <div class="pagination-controls">
          <button class="prev">❮ &nbsp;</button>
          <button class="one">1</button>
          <button>2</button>
          <button>...</button>
          <button>9</button>
          <button>10</button>
          <button class="next">❯ &nbsp;</button>
        </div>
      </div>
    </table>
    <house-footer />
  </div>
</template>

<script>
export default {}
</script>

<style>
table {
  border-spacing: 0px;
  width: 90%;
  background: #fff;
  margin-left: 34px;
  margin-bottom: 30px;
}
.table-data {
  background: #f5f8ff;
}
.data {
  padding: 10px 20px;
}
td {
  padding: 15px 25px 15px 30px;

  text-align: left;
}
th {
  padding: 15px 0px 15px 30px;
  text-align: left;
}
.customer {
  color: #f7941d;
}
.pagination-container {
  /* background: green; */
}
.pagination-controls {
  display: flex;
  justify-content: flex-end;
  background: red;
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
  padding: 1px 3px;
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
