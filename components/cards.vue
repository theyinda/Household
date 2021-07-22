<template>
  <div class="card-container">
    <div class="card">
      <div class="card__content">
        <div>
          <img src="@/assets/images/card1.svg" />
        </div>
        <div>
          <h4>830</h4>
          <p>Total Candidates</p>
        </div>
      </div>
    </div>

    <div class="card card--two">
      <div class="card__content">
        <div>
          <img src="@/assets/images/card2.svg" />
        </div>
        <div>
          <h4>280</h4>
          <p>Total Customers</p>
        </div>
      </div>
    </div>

    <div class="card">
      <div class="card__content">
        <div>
          <img src="@/assets/images/card3.svg" />
        </div>

        <div>
          <h4>200</h4>
          <p>Total Requests</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style >
.card-container {
  display: flex;
  width: 90%;
  margin-left: 34px;
}
.card {
  display: flex;
  width: 100%;
  height: 144px;
  margin: 39px auto 129px auto;
  background: #ffffff;
  border: 1px solid #ebf1f4;
  box-shadow: 0px 4px 16px rgba(235, 241, 244, 0.6);
}
.card--two {
  margin-left: 16px;
  margin-right: 16px;
}
.card__content {
  display: flex;
  margin: auto 0;
  /* background: red; */
}
.card img {
  margin: 0 24px;
}
</style>
