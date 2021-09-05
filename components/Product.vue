<template>
  <section class="product_bg-color">
    <div class="product_container section-inner">
      <h2 class="product_title">PRODUCT</h2>
      <div class="product_infomation-txt product_bar">
        PRODUCT&nbsp;INFORMATION
      </div>
      <div class="product_dummy-txt-group">
        <h3 class="product_dummy-txt-1">
          この文章はダミーです。
        </h3>
        <div class="product_dummy-txt-2">
          この文章はダミーです。文字の大きさ、量、字間、行間等を確認を確認するために入れています。
        </div>
      </div>
      <div class="product_list-group">
        <div
          class="product_list-content"
          v-for="product in productList"
          :key="product.img"
        >
          <div class="product_list">
            <img style="width: 100%;" :src="product.image" alt="" />
          </div>
          <div class="product_list-title">{{ product.title }}</div>
          <div class="product_list-text">{{ product.description }}</div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.product_container {
  padding: 7rem 2rem;
}
.product_list-title {
  font-size: 1.6rem;
  margin-bottom: 2rem;
}
.product_list-text {
  font-size: 1.2rem;
  line-height: 2rem;
  letter-spacing: 0.02rem;
}
.product_bg-color {
  position: relative;
}
.product_bg-color::before {
  position: absolute;
  z-index: -1;
  display: block;
  content: "";
  background: #45556a;
  top: 0;
  bottom: 0;
  right: 0;
  left: 0;
  width: 100%;
  height: 20.5%;
}
.product_list-content {
  margin: 5rem 0;
}
.product_title {
  font-weight: 500;
  line-height: 1.25;
  color: #fff;
  margin: 0 0 1.2rem 1rem;

  font-size: 4.2rem;
}

.product_bar {
  font-weight: 500;
  position: relative;
  line-height: 1.25;
  letter-spacing: 0.08em;
  color: rgba(255, 255, 255, 0.5);
}

.product_infomation-txt {
  font-size: 1.2rem;
  margin: 0 0 3rem 1rem;
}

.product_bar::before {
  position: absolute;
  top: 50%;
  display: block;
  width: 2rem;
  height: 1px;
  content: "";
  background: #fff;
  left: -4rem;
}
.product_dummy-txt-1 {
  line-height: 1.25;
  color: #fff;
  font-size: 2.1rem;
  margin-bottom: 2rem;
}

.product_dummy-txt-2 {
  font-size: 1.6rem;
  color: #fff;
  margin-bottom: 4rem;
}
.product_list img {
  margin-bottom: 3rem;
}
@media only screen and (min-width: 768px) {
  .product_list-text {
    font-size: 1.3rem;
    line-height: 2.7rem;
    letter-spacing: 0.1rem;
  }
  .product_bg-color::before {
    height: 37%;
  }
  .product_title {
    font-size: 6rem;
    margin: 0 0 1.2rem 0;
  }

  .product_bar::before {
    transform: translate(calc(-100% - 1.8rem), -50%);
    left: 0;
  }
  .product_dummy-txt-1 {
    width: 100%;
    font-size: 2.4rem;
  }

  .product_dummy-txt-2 {
    margin-bottom: 6rem;
    line-height: 2;
  }

  .product_list-group {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
  .product_list-content {
    width: 47.5%;
    margin: 5rem 0;
  }

  .product_infomation-txt {
    margin: 0 0 3.5rem 0;
  }
}
</style>

<script lang="ts">
import { Vue, Component } from "nuxt-property-decorator";

@Component({})
export default class extends Vue {
  productList = [
    {
      image: require("static/product-img/product-img1.jpg"),
      title: "ダミーダミーダミー",
      description:
        "この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。この文章はダミーです。"
    },
    {
      image: require("static/product-img/product-img2.jpg"),
      title: "ダミーダミーダミー",
      description:
        "この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。この文章はダミーです。"
    },
    {
      image: require("static/product-img/product-img3.jpg"),
      title: "ダミーダミーダミー",
      description:
        "この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。この文章はダミーです。"
    },
    {
      image: require("static/product-img/product-img4.jpg"),
      title: "ダミーダミーダミー",
      description:
        "この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。この文章はダミーです。"
    }
  ];

  nameChange() {}
}
</script>
