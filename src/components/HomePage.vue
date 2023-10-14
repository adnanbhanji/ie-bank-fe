<template>
  <div class="homepage">
    <img
      src="https://www.tautdanning.no/wp-content/uploads/2018/12/IE-University-logo.png"
      alt="Banco Sabadell"
      class="logo"
    />

    <h1>Welcome to <span>IE Bank Corp.</span></h1>
    <h2>Invest in your tomorrow, today!</h2>

    <div class="button-container">
      <router-link to="/skull">
        <button type="button" class="btn btn-primary">Test Connection</button>
      </router-link>

      <router-link to="/accounts">
        <button type="button" class="btn btn-primary">View Accounts</button>
      </router-link>
    </div>

    <div class="social-media">
      <br />
      <h3>Stay connected with us on social media:</h3>
      <a href="https://www.instagram.com/adnanintech" target="_blank">
        <img
          src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/Instagram_icon.png/600px-Instagram_icon.png?20200512141346"
          alt="Instagram"
        />
      </a>
      <a href="https://www.linkedin.com/in/adnanbhanji/" target="_blank">
        <img
          src="https://cdn1.iconfinder.com/data/icons/logotypes/32/circle-linkedin-512.png"
          alt="LinkedIn"
        />
      </a>
      <a href="https://github.com/adnanbhanji" target="_blank">
        <img
          src="https://cdn-icons-png.flaticon.com/512/25/25231.png"
          alt="Twitter"
        />
      </a>
    </div>
  </div>
</template>

<style scoped>
.homepage {
  text-align: center;
  padding: 20px;
  padding-top: 70px;
  /* background-image: url("https://wallpaper.dog/large/17062513.jpg"); */
  height: 100vh;
}

.logo {
  max-width: 200px;
}

h1 {
  font-size: 28px;
  padding: 5px;
  margin: 10px 0;
}
span {
  background: linear-gradient(90deg, rgb(16, 194, 218), rgb(8, 79, 161));
  -webkit-background-clip: text;
  color: transparent;
}

h2 {
  font-size: 19px;
  margin-top: 10px;
  margin-bottom: 30px;
  /* background: linear-gradient(90deg, rgb(16, 194, 218), rgb(8, 79, 161));
  -webkit-background-clip: text;
  color: transparent; */
}

.button-container {
  display: flex;
  justify-content: center;
  gap: 20px;
}

.btn {
  background-color: #007bff;
  color: #fff;
  font-size: 18px;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.btn:hover {
  background-color: #0056b3;
}

.social-media {
  margin-top: 20px;
}

.social-media h3 {
  font-size: 16px;
}

.social-media a {
  margin: 0 10px;
  text-decoration: none;
}

.social-media img {
  margin: 10px 0;
  max-width: 40px;
}
</style>
