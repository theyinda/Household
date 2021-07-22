<template>
  <div class="container">
    <householdheader />
    <div class="customer-dashboard">
      <sidenav />
      <div class="customer-dashboard__item">
        <section class="dashboard-view">
          <div class="dashboard-view-container">
            <h4>Welcome Back, Oluwaseun</h4>
            <p class="title">You have 19 new requests and other tasks to do</p>
          </div>

          <cards />

          <div class="table-header">
            <div class="table__text">
              <p>Resent Sign ups</p>
            </div>

            <div class="tabs">
              <div
                :class="
                  activeTab.includes('customer-tab') ? 'active' : 'inactive'
                "
                class="customer-tab"
                @click="activeTab = 'customer-tab'"
              >
                Customer
              </div>
              <div
                :class="
                  activeTab.includes('candidates-tab') ? 'active' : 'inactive'
                "
                class="candidates-tab"
                @click="activeTab = 'candidates-tab'"
              >
                Candidates
              </div>
            </div>
          </div>

          <table>
            <div
              v-show="activeTab == 'customer-tab'"
              class="tab-1 customer-tab"
            >
              <thead>
                <tr class="table-data">
                  <th>User ID</th>
                  <th>Registration Date</th>
                  <th>Full Name</th>
                  <th>Email Address</th>
                  <th>User Type</th>
                </tr>
              </thead>

              <tr
                v-for="records in tableData"
                :key="records.userId"
                class="table-body"
              >
                <td>{{ records.userId }}</td>
                <td>{{ records.regDate }}</td>
                <td>{{ records.fullName }}</td>
                <td>{{ records.email }}</td>
                <td class="user">
                  {{ records.userType }}
                </td>
              </tr>
            </div>
          </table>

          <div v-show="activeTab == 'candidates-tab'" class="tab-2">
            <table-data />
          </div>
        </section>
        <householdfooter />
      </div>
    </div>
  </div>
</template>

<script>
export default {
 
  data() {
    return {
      activeTab: 'customer-tab',
      tableData: [
        {
          userId: '#ND1283',
          regDate: '23.04.2020',
          fullName: 'Abdul Ifeoma',
          email: 'amaranth@outlook.com',
          userType: 'Customer',
        },
        {
          userId: '#ND1283',
          regDate: '23.04.2020',
          fullName: 'Abdul Ifeoma',
          email: 'amaranth@outlook.com',
          userType: 'Customer',
        },
        {
          userId: '#ND1283',
          regDate: '23.04.2020',
          fullName: 'Abdul Ifeoma',
          email: 'amaranth@outlook.com',
          userType: 'Customer',
        },
        {
          userId: '#ND1283',
          regDate: '23.04.2020',
          fullName: 'Abdul Ifeoma',
          email: 'amaranth@outlook.com',
          userType: 'Customer',
        },
        {
          userId: '#ND1283',
          regDate: '23.04.2020',
          fullName: 'Abdul Ifeoma',
          email: 'amaranth@outlook.com',
          userType: 'Customer',
        },
        {
          userId: '#ND1283',
          regDate: '23.04.2020',
          fullName: 'Abdul Ifeoma',
          email: 'amaranth@outlook.com',
          userType: 'Customer',
        },
      ],
    }
  },
}
</script>

<style scoped>
.container {
  /* background: red; */
  margin: 20px auto;
  width: 100%;
}
.customer-dashboard {
  width: 95%;
  display: flex;
  margin: 20px auto;
  background: green;
}
.dashboard-view-container {
  margin-top: 15px;
  margin-left: 34px;
}
.dashboard-view-container h4 {
  font-style: normal;
  font-weight: 500;
  font-size: 36px;
  align-items: center;
  color: #000000;
}
.dashboard-view-container p {
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  align-items: center;
  color: #717f88;
  padding-top: 15px;
}
.table-header {
  width: 90%;
  background: #fff;
  display: flex;
  margin-left: 34px;
  justify-content: space-between;
}
table {
  border-spacing: 0px;
  width: 90%;
  background: red;
  background: #fff;
  margin-left: 34px;
  margin-bottom: 30px; 
   margin-top: 50px;
}
.table__text {
  text-align: center;
  padding-top: 10px;
  padding-left: 30px;
}

/* TABS  */

.tabs {
  background-color: #f9fafb;
  display: flex;
  /* width: 400px; */
  border-radius: 8px;
  border: 1px solid #e1edfe;
}

.customer-tab {
  border-radius: 8px 0 0 8px;
}
.candidates-tab {
  border-radius: 0 8px 8px 0;
}

.tabs div {
  padding: 12px 25px;
  font-size: 14px;
  width: 200px;
  text-align: center;
  border: none;
  background-color: transparent;
  cursor: pointer;
}

.tabs div:hover {
  background-color: #00a69d !important;
  color: white;
}

.active {
  background-color: #00a69d !important;
  color: white;
}

.user {
  color: #f7941d;
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
</style>
