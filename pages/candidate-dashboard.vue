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

            <div class="table__btns">
              <button>Customer</button>
              <button class="btn-2">Candidates</button>
            </div>
          </div>
          <table-data />
           <householdfooter />
        </section>
      </div>
    </div>
  </div>
</template>

<script>
import householdheader from '../components/householdheader.vue'
import householdfooter from '../components/householdfooter.vue'
import Sidenav from '../components/sidenav.vue'

export default {
  components: { householdheader, Sidenav, householdfooter },
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

a {
  text-decoration: none;
}

ul {
  list-style: none;
}

i,
a,
button {
  cursor: pointer;
}

.container {
  margin: 20px auto;
  width: 100%;
}

.customer-dashboard {
  display: flex;
  margin: 20px auto;
}

.dashboard-view-container {
  margin-top: 30px;
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
.table__text {
  text-align: center;
  padding-top: 10px;
  padding-left: 30px;
}

.table__btns button {
  background: #00a69d;
  border-radius: 5.85013px 0px 0px 5.85013px;
  font-style: normal;
  border-style: none;
  font-weight: normal;
  padding: 11px 20px;
  font-size: 13.1628px;
  line-height: 16px;
  text-align: center;
  color: #ffffff;
}
.table__btns .btn-2 {
  background: #f9fafb;
  color: #909197;
  border: 0.731266px solid #e1edfe;
  border-radius: 0px 5.85013px 5.85013px 0px;
}
</style>
