<template>
  <div>
    <div class="box"></div>
    <div>
      <p>{{ product_name }}</p>
      <p>$ {{ price }}</p>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    product_name: String,
    price: Number,
  },
};
</script>
<style scoped>
.box {
  height: 20rem;
  width: 20rem;
  background-color: gray;
  margin-left: 10px;
  margin-right: 10px;
  margin-top: 5px;
}
p {
  font-size: 0.875em;
  margin-left: 10px;
  margin-right: 10px;
  margin-top: 10px;
}
</style>
