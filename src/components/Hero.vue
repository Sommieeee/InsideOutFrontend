<template>
  <div class="main-div">
    <div class="text">
      <h2>Made for the Season</h2>

      <div class="first">
        <p>Introducing Inside Out.</p>
      </div>
      <div class="second">
        <p>Our latest collection.</p>
      </div>
      <button>SHOP</button>
    </div>
    <div class="img">
      <img src="@/assets/images/rings.jpg" />
    </div>
    <!-- <div class="img">
      <img src="@/assets/images/bracelet2.png" />
    </div> -->
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
.main-div {
  display: flex;
  justify-content: space-evenly;
  height: 60vh;
  width: 100%;
}
.text {
  display: flex;
  flex-direction: column;
  height: 100%;
  justify-content: flex-end;
  padding-bottom: 4rem;
  /* padding-left: 4rem; */
}
img {
  height: 100%;
  width: auto;
  margin-top: 2em;
  /* padding-right: 2rem; */
}
h2 {
  font-size: 24px;
  display: flex;
  justify-content: center;
  /* margin-top: 10px; */
  margin-left: 40px;
}
p {
  margin-top: 12px;
  line-height: 15px;
}
button {
  background-color: black;
  border: none;
  color: white;
  padding: 10px 16px;
  margin-left: 80px;
  margin-right: 50px;
  margin-top: 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  display: flex;
  justify-content: center;
  /* margin-top: 10px; */
  /* margin-left: 40px; */
}
.first {
  display: flex;
  justify-content: center;
  /* margin-top: 10px; */
  margin-left: 40px;
}
.second {
  display: flex;
  justify-content: center;
  /* margin-top: 10px; */
  margin-left: 40px;
}
</style>
