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

      <tr v-for="records in tableData" :key="records.userId" class="table-body">
        <td class="">{{ records.userId }}</td>
        <td class="">{{ records.regDate }}</td>
        <td class="">{{ records.fullName }}</td>
        <td class="">{{ records.email }}</td>
        <td class="user">
          {{ records.userType }}
        </td>
      </tr>
    </table>
    <house-footer />
  </div>
</template>

<script>
export default {
  data() {
    return {
      tableData: [
        {
          userId: '#ND1283',
          regDate: '23.04.2020',
          fullName: 'Abdul Ifeoma',
          email: 'amaranth@outlook.com',
          userType: 'Candidates',
        },
        {
          userId: '#ND1283',
          regDate: '23.04.2020',
          fullName: 'Abdul Ifeoma',
          email: 'amaranth@outlook.com',
          userType: 'Candidates',
        },
        {
          userId: '#ND1283',
          regDate: '23.04.2020',
          fullName: 'Abdul Ifeoma',
          email: 'amaranth@outlook.com',
          userType: 'Candidates',
        },
        {
          userId: '#ND1283',
          regDate: '23.04.2020',
          fullName: 'Abdul Ifeoma',
          email: 'amaranth@outlook.com',
          userType: 'Candidates',
        },
        {
          userId: '#ND1283',
          regDate: '23.04.2020',
          fullName: 'Abdul Ifeoma',
          email: 'amaranth@outlook.com',
          userType: 'Candidates',
        },
        {
          userId: '#ND1283',
          regDate: '23.04.2020',
          fullName: 'Abdul Ifeoma',
          email: 'amaranth@outlook.com',
          userType: 'Candidates',
        },
      ],
    }
  },
}
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

td {
  padding: 15px 25px 15px 30px;
  text-align: left;
}
th {
  padding: 15px 20px 15px 30px;
  text-align: left;
}
.user {
  /* color: #f7941d; */
  color: #00a69d;
}
</style>
