<template>
  <div class="homepage">
    <img
      src="data:image/png;base64,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"
      alt="Banco Sabadell"
      class="logo"
    />

    <h1>Welcome to <span>Banco Sabadell</span></h1>
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
