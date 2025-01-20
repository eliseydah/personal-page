<script setup lang="ts"></script>
<template>
  <section class="container-sign">
    <p class="text-front">ABOUT ME</p>
    <p class="text-back">ABOUT ME</p>
  </section>
  <section>
    <div class="contain">
      <div>
        <img src="../assets/forest.jpg" width="250" height="300" />
      </div>
      <div class="text-box">
        <h3>Hello, world!</h3>
        <h5>I'm Daria Eliseeva</h5>
        <p>Enthusiastic Frontend Developer.</p>
        <section>
          <p>Birthday: <span>16.12.1998</span></p>
          <p>Phone: <span></span></p>
          <p>E-mail: <span> eliseydah@gmail.com</span></p>
          <p>Live in: <span> Berlin</span></p>
          <p>Language:<span> English, Russian</span></p>
          <button class="downloadCv">Resume</button>
        </section>
      </div>
    </div>
  </section>
</template>
<style>
.container-sign {
  position: relative;
  height: 10vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.text-back {
  position: absolute;
  font-size: 36px;
  font-weight: bold;
  color: rgba(211, 211, 211, 0.08);
  z-index: 1; /* Элемент под другим */
}

.text-front {
  position: absolute;
  font-size: 16px;
  font-weight: bold;
  color: rgba(170, 215, 255, 1);
  z-index: 2; /* Элемент над другим */
}
.title {
  font-size: 1.2rem;
  text-align: center;
  margin-top: 2rem;
  color: rgba(170, 215, 255, 1);
  text-decoration: underline;
  position: relative;
}
.backgroundTitle {
  font-size: 1.2rem;
  text-align: center;
  color: darkblue;
  margin-bottom: 5rem;
  text-decoration: underline;
  position: absolute;
}
.contain {
  font-size: 1.5rem;
  background-color: rgba(240, 248, 255, 0.8);
  padding: 3rem 3rem;
  display: flex;
  gap: 2rem;
  justify-content: space-around;
  align-items: center;
  height: 50vh;
}
.text-box {
  display: flex;
  flex-direction: column;
  font-size: 1.2rem;
}
.downloadCv {
  margin-top: 2rem;
  width: 10rem;
  padding: 1rem 3rem;
  background-color: rgba(240, 242, 243, 0.45);
  color: darkblue;
  border: 0;
  border-radius: 2rem;
}
.downloadCv:hover {
  background-color: rgba(240, 248, 255, 0.65);
}
h3 {
  align-self: center;
  font-size: 2rem;
  color: black;
  font-family: 'Times New Roman', Times, serif;
}
h5 {
  font-size: 1.5rem;
  color: rgb(0, 140, 216);
  font-weight: bold;
}
</style>
