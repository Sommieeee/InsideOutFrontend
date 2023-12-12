<template>
  <div>
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"
    />
    <Header/>
    <Hero />
    <div>
      <h3>New Releases</h3>
    </div>
    <div class="flex">
      <ProductPriceCard
        v-for="(unit, i) in productListArr"
        :key="i"
        :product_name="unit.product_name"
        :price="unit.price"
      />
    </div>
  </div>
  <div>
    <h3>Top Picks</h3>
    <div class="flex">
      <TopPicksCard
        v-for="(unit, i) in productList"
        :key="i"
        :name="unit.name"
        :product_price="unit.product_price"
      />
    </div>
    <div class="mailing">
      <h3>Own that runway</h3>
    </div>
    <div class="first">
      <p>Receive updates about new styles and</p>
    </div>
    <div class="second">
      <p>promotions</p>
    </div>

    <button>Join mailing list</button>
    <div class="footer">
      <div class="container">
        <div class="row">
          <div class="footer-col">
            <h4>My Account</h4>
            <ul>
              <li>
                <a href="#">Sign In</a>
              </li>
              <li>
                <a href="#">Register</a>
              </li>
              <li>
                <a href="#">Order status</a>
              </li>
            </ul>
          </div>
          <div class="footer-col">
            <h4>Help</h4>
            <ul>
              <li>
                <a href="#">Shipping</a>
              </li>
              <li>
                <a href="#">Returns</a>
              </li>
              <li>
                <a href="#">Register</a>
              </li>
            </ul>
          </div>
          <div class="footer-col">
            <h4>About</h4>
            <ul>
              <li>
                <a href="#">Our story</a>
              </li>
              <li>
                <a href="#">Media</a>
              </li>
              <li>
                <a href="#">Sustainability</a>
              </li>
            </ul>
          </div>
          <div class="footer-col">
            <h4>Legal</h4>
            <ul>
              <li>
                <a href="#">Terms of use</a>
              </li>
              <li>
                <a href="#">Terms of sale</a>
              </li>
              <li>
                <a href="#">Privacy policy</a>
              </li>
            </ul>
          </div>
          <div class="footer-col">
            <h4>Follow Us</h4>
            <div class="social-links">
              <a href="#"><i class="fab fa-facebook-f"></i></a>
              <a href="#"><i class="fab fa-instagram"></i></a>
              <a href="#"><i class="fab fa-twitter"></i></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Header from "../components/Header.vue";
import Hero from "../components/Hero.vue";
import ProductPriceCard from "../components/ProductPriceCard.vue";
import TopPicksCard from "../components/TopPicksCard.vue";

export default {
  components: {
    Header,
    ProductPriceCard,
    Hero,
    TopPicksCard,
  },
  data() {
    return {
      productListArr: [
        {
          product_name: "Product Name",
          price: 5,
        },
        {
          product_name: "Product Name",
          price: 5,
        },
        {
          product_name: "Product Name",
          price: 5,
        },
        {
          product_name: "Product Name",
          price: 5,
        },
        {
          product_name: "Product Name",
          price: 5,
        },
        {
          product_name: "Product Name",
          price: 5,
        },
      ],
      productList: [
        {
          name: "Product Name",
          product_price: 5,
        },
        {
          name: "Product Name",
          product_price: 5,
        },
        {
          name: "Product Name",
          product_price: 5,
        },
        {
          name: "Product Name",
          product_price: 5,
        },
        {
          name: "Product Name",
          product_price: 5,
        },
        {
          name: "Product Name",
          product_price: 5,
        },
        {
          name: "Product Name",
          product_price: 5,
        },
        {
          name: "Product Name",
          product_price: 5,
        },
      ],
    };
  },
};
</script>

<style scoped>
.flex {
  display: flex;
  overflow-x: auto;
  margin-left: 20px;
  margin-top: 5px;
}
h3 {
  font-size: 30px;
  margin-left: 30px;
  margin-top: 50px;
  font-weight: 700;
}
.mailing {
  display: flex;
  justify-content: center;
}
.first {
  display: flex;
  justify-content: center;
  margin-top: 10px;
  margin-left: 40px;
}
.second {
  display: flex;
  justify-content: center;
}
button {
  background-color: white;
  border-color: black;
  color: black;
  padding: 18px 40px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 10px auto;
  display: block;
}
.container {
  max-width: 1170px;
  margin: auto;
}
.row {
  display: flex;
  flex-wrap: wrap;
}
ul {
  list-style: none;
}
.footer {
  background-color: black;
  padding: 40px 0;
  margin-top: 70px;
}
.footer-col {
  width: 25%;
  padding: 0 15px;
  margin-top: 20px;
}
.footer-col h4 {
  font-size: 18px;
  color: #ffffff;
  text-transform: capitalize;
  margin-bottom: 35px;
  font-weight: 500;
  position: relative;
}
.footer-col h4::before {
  content: "";
  position: absolute;
  left: 0;
  bottom: -10px;
  background-color: white;
  height: 2px;
  box-sizing: border-box;
  width: 50px;
}
.footer-col ul li:not(:last-child) {
  margin-bottom: 10px;
}
.footer-col ul li a {
  font-size: 16px;
  text-transform: capitalize;
  color: #ffffff;
  text-decoration: none;
  font-weight: 300;
  color: #bbbbbb;
  display: block;
  transition: all 0.3s ease;
}
.footer-col ul li a:hover {
  color: #ffffff;
  padding-left: 8px;
}
.footer-col .social-links a {
  display: inline-block;
  height: 40px;
  width: 40px;
  background-color: rgba(255, 255, 255, 0.2);
  margin: 0 10px 10px 0;
  text-align: center;
  line-height: 40px;
  border-radius: 50%;
  color: #ffffff;
  transition: all 0.5s ease;
}
.footer-col .social-links a:hover {
  color: #24262b;
  background-color: #ffffff;
}
</style>
