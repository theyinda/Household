<template>
  <div class="login">
    <div class="login__item">
      <div class="logo-img">
        <img src="../assets/images/main_logo.svg" alt="logo" />
        <p>Good help, Better Life</p>
      </div>

      <div class="polygons">
        <img src="../assets/images/polygon2.svg" class="polygon" />
        <img src="../assets/images/polygon1.svg" class="polygon1" />
      </div>
    </div>

    <div class="login__details">
      <div class="login__text">
        <h4>Welcome Back!</h4>
        <p>Login with your account details to continue.</p>
      </div>

      <div class="login__input">
        <form>
          <label>Email Address</label> <br />
          <input type="text" class="" placeholder="placeholder@mail.com" />
          <br />
          <label>Password</label> <br />
          <input
            type="text"
            class=""
            placeholder="***************************"
          />

          <div class="c">
            <nuxt-link to="/forgot-password" class="link"
              >Forgot password?</nuxt-link
            >
          </div>
          <button class="login__button">Login</button>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.login {
  display: flex;
  width: 100%;
  background-color: #e5e5e5;
  background: red;
}
.login__item {
  background: linear-gradient(153.01deg, #006838 0.64%, #00a69d 99.19%);
}
.login__item .logo-img {
  display: block;
  margin: 234px auto 30px auto;

  width: 50%;
}
.login__item .logo-img p {
  font-style: normal;
  font-weight: normal;
  font-size: 24px;
  line-height: 18px;
  text-align: center;

  color: #ffffff;
}
.polygons {
  position: relative;
}
.polygon1 {
  position: absolute;
  bottom: 0px;
  left: 0px;
}
.login__details {
  background: #fff;
  width: 742px;
}
.login__text {
  margin-top: 100px;
  margin-bottom: 50px;
  text-align: center;
}
.login__text h4 {
  font-weight: 600;
  font-size: 24px;
  line-height: 29px;
  color: #f7941d;
}
.login__text p {
  font-size: 18px;
  line-height: 18px;
  color: #57565c;
  padding-top: 18px;
}
.login__input {
  width: 85%;
  padding-left: 50px;
  margin: 0 auto;
}
.login__input label {
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 18px;
  color: #042538;
}
.login__input input {
  background: #ffffff;
  border: 1px solid #c4c4c4;

  width: 88%;
  margin: 10px 0;
  padding: 10px 15px;
  border-radius: 8px;
}
.login__button {
  background: #00a69d;
  border: 2px solid #00a69d;
  box-sizing: border-box;
  border-radius: 8px;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 19px;
  text-align: center;
  color: #ffffff;
  width: 88%;
  padding: 10px 15px;
  margin: 65px 0;
}
.c {
  display: flex;
  justify-content: flex-end;
  text-decoration: none;
  width: 88%;
}
.link {
  font-weight: 500;
  font-size: 14px;
  line-height: 18px;
  text-align: right;
  color: #00a69d;
}
</style>
