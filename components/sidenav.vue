<template>
  <div class="customer-dashboard__sidebar">
    <nav class="sidebar">
      <ul class="side-nav">
        <li class="side-nav_item">
          <img src="../assets/images/home.svg" alt="logo" />
          <a href="#" class="side-nav_link">
            <span>Dashboard</span>
          </a>
        </li>

        <li class="side-nav_item">
          <img src="../assets/images/customers.svg" alt="logo" />
          <a href="#" class="side-nav_link">
            <span>Customers</span>
          </a>
        </li>

        <li class="side-nav_item">
          <img src="../assets/images/candidates.svg" alt="logo" />
          <a href="#" class="side-nav_link">
            <span>Candidates</span>
          </a>
        </li>
        <li class="side-nav_item">
          <img src="../assets/images/requests.svg" alt="logo" />
          <a href="#" class="side-nav_link">
            <span>Requests</span>
          </a>
        </li>
        <li class="side-nav_item elephant">
          <img src="../assets/images/payment.svg" alt="logo" />
          <a href="#" class="side-nav_link">
            <span>Payment</span>
          </a>
        </li>

        <li class="side-nav_item">
          <img src="../assets/images/reviews.svg" alt="logo" />
          <a href="#" class="side-nav_link">
            <span>Reviews</span>
          </a>
        </li>

        <li class="side-nav_item">
          <img src="../assets/images/settings.svg" alt="logo" />
          <a href="#" class="side-nav_link">
            <span>Settings</span>
          </a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {}
</script>

<style>
.customer-dashboard__sidebar {
  background: #fff;
  width: 245px;
}
.customer-dashboard__item {
  background: #f3f6f8;
  width: 100%;
}
.side-nav_item {
  margin-top: 40px;
  text-align: left;
  margin-left: 44px;
}
.side-nav_item span {
  color: #6f8a9c;
}
.side-nav_item img {
  margin: 0 15px 0 0px;
}

.side-nav_item:hover {
  /* transform: matrix(1, 0, 0, 1, 0, 0);
  background: rgba(4, 37, 56, 0.3);
  opacity: 0.2; */
  color: #010025;
  /* height: 60px; */
}
.side-nav_item span:hover {
  color: #010025;
  transform: matrix(1, 0, 0, 1, 0, 0);
  background: rgba(4, 37, 56, 0.3);
  opacity: 0.2;
  color: #010025;
  height: 60px;
  width: 400px;
}
</style>
