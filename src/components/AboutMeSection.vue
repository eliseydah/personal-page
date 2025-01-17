<script setup lang="ts"></script>
<template>
  <section>
    <p class="title">ABOUT ME</p>
    <div class="contain">
      <div><img src="./forest.jpg;" alt="" width="50" height="60" /></div>
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
.title {
  font-size: 1.2rem;
  text-align: center;
  margin-top: 2rem;
  color: darkblue;
  text-decoration: underline;
  margin-bottom: 5rem;
}
.contain {
  font-size: 1.5rem;
  background-color: rgba(240, 248, 255, 0.35);
  padding: 3rem 3rem;
  display: flex;
  gap: 2rem;
  justify-content: space-between;
  align-items: center;
  height: 50vh;
  /* flex-direction: column; */
  gap: 2rem;
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
</style>
