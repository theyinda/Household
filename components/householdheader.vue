<template>
  <div class="header">
    <div class="header__logo">
      <img src="@/assets/images/logo.svg" alt="logo" />
      <h5>Dashboard</h5>
    </div>

    <div class="header__img">
      <img src="@/assets/images/notification.svg" alt="" />
      <img src="@/assets/images/profile.svg" alt="" />
      <img src="@/assets/images/arrow.svg" alt="" />
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.header{
  display: flex;
  justify-content: space-between;
  margin: 44px;
}
.header__logo{
  display: flex;
  /* justify-content: space-between; */
 
}
.header__logo h5{
  text-align: center;
  padding-left: 80px;
  padding-top: 12px;
}
.header__img{
  display: flex;
  justify-content: space-evenly;
  margin-left: 20px;
 
}
.header__img img{
  margin-left: 20px;
}
</style>
