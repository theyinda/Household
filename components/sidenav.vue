<template>
  <div class="customer-dashboard__sidebar">
    <nav class="sidebar">
        <nuxt-link to="/"
        ><div class="side-nav_item">
          <img src="../assets/images/home.svg" alt="icon" />
          <p>Dashboard</p>
        </div></nuxt-link
      >
        

        <nuxt-link to="/customers"
        ><div class="side-nav_item">
          <img src="../assets/images/customers.svg" alt="icon" />
          <p>Customers</p>
        </div></nuxt-link
      >

        <nuxt-link to="/candidates"
        ><div class="side-nav_item">
          <img src="../assets/images/candidates.svg" alt="icon" />
          <p>Candidates</p>
        </div></nuxt-link
      >
        <nuxt-link to="/requests"
        ><div class="side-nav_item">
          <img src="../assets/images/requests.svg" alt="icon" />
          <p>Requests</p>
        </div></nuxt-link
      >
        <nuxt-link to="/payment"
        ><div class="side-nav_item">
          <img src="../assets/images/payment.svg" alt="icon" />
          <p>Payment</p>
        </div></nuxt-link
      >

        <nuxt-link to="/reviews"
        ><div class="side-nav_item">
          <img src="../assets/images/reviews.svg" alt="icon" />
          <p>Reviews</p>
        </div></nuxt-link
      >

        <nuxt-link to="/settings"
        ><div class="side-nav_item">
          <img src="../assets/images/settings.svg" alt="icon" />
          <p>Settings</p>
        </div></nuxt-link
      >
  
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

  /* position: fixed;
 padding-top: 74px;
  height: 900px; */
}
.side-nav_item {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
  height: 60px;
  cursor: pointer;
}
.side-nav_item img {
  padding: 20px 20px 20px 32px;
}

.side-nav_item p {
  color: #6f8a9c;
  width: 100%;
  padding: 21px 16px;
  font-size: 15px;
  margin: 0;
}

a.nuxt-link-exact-active .side-nav_item,
a:hover .side-nav_itemu {
  background-color: rgba(4, 37, 56, 0.076);
}

a.nuxt-link-exact-active p,
a:hover p {
  color: #010025;
  font-weight: 600;
}

a.nuxt-link-exact-active img,
a:hover img {
  background-color: #010025;
  border-radius: 0 20px 20px 0;
}

</style>
