<template>
  <header>
    <div class="header-content">
      <div class="header-title">日本ALO音楽研究所</div>
      <div class="header-contents">
        <div class="header_tel-icon">
          <img src="icon/header-sp_tel-icon.png" alt="header-sp_tel-icon" />
        </div>
        <div class="header_email-icon">
          <img src="icon/header-sp_email-icon.png" alt="header-sp_email-icon" />
        </div>
        <div class="header_tel-group">
          <dl class="tel-group-content">
            <dt>TEL</dt>
            <dd>0120-00-0000</dd>
          </dl>
          <div class="tel-group-open">
            10:00〜18:00&nbsp;土日・祝日・年末年始除く
          </div>
        </div>

        <div class="header-tel-icon"></div>
        <div class="header-contact">
          <a href="#form">
            お問い合わせ
          </a>
        </div>
        <button class="header-hum-menu" @click="openMenu">
          <span>MENU</span>
          <i></i>
        </button>
      </div>
    </div>
    <div v-show="isOpened" class="menu">
      <div class="menu-header">
        <p class="title-in-menu">日本ALO音楽研究所</p>
        <button class="close" @click="openMenu">
          <i></i>
        </button>
      </div>
      <div class="menu-list">
        <ul>
          <li v-for="menu in menuList" :key="menu.id">
            {{ menu }}
          </li>
        </ul>
      </div>
      <div class="mail-contact">
        <div>
          <div class="header_tel-icon">
            <img src="icon/header-sp_tel-icon.png" alt="header-sp_tel-icon" />
          </div>
          <div>メールでのお問い合わせ</div>
        </div>
        <div class="menu-contact">
          <a href="#form">
            お問い合わせ
          </a>
        </div>
      </div>
      <div class="tel-contact">
        <div>
          <div class="header_tel-icon">
            <img src="icon/header-sp_tel-icon.png" alt="header-sp_tel-icon" />
          </div>
          <div>お電話でのお問い合わせ</div>
        </div>

        <div>0120-00-0000</div>
        <p>10:00〜18:00 土日・祝日・年末年始除く</p>
      </div>
    </div>
  </header>
</template>

<style scoped>
.header_tel-icon,
.header_email-icon {
  margin-right: 1.8rem;
}
.header_email-icon img {
  width: 100%;
  height: 2.7rem;
}
.header_tel-icon img {
  width: 100%;
  height: 2.5rem;
}
.header_tel-group {
  display: none;
}
.header-content {
  background: #fff;
  display: flex;
  position: fixed;
  top: 0;
  z-index: 10;
  justify-content: space-between;
  width: 100%;
  margin: 0 0 0 auto;
  align-items: center;
  /* height: 6rem; */
}
.header-contact {
  display: none;
}
.header-content,
.header-contents {
  color: #000;
}
.header-title {
  font-size: 1.5rem;
  padding-left: 2rem;
  width: 18.8rem;
}

/* ------------------------------------------ */
.header-contents {
  display: flex;
  z-index: 1;
  align-items: center;
  justify-content: flex-end;
}
.tel-group-content {
  display: flex;
  align-items: center;
  margin-bottom: 0.6rem;
  line-height: 1;
  letter-spacing: 0.1em;
  margin-top: 0;
}

.header-hum-menu i {
  position: relative;
  display: block;
  margin-bottom: auto;
  width: 2.6rem;
  height: 0.8rem;
}

.header-hum-menu {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  padding-bottom: 1rem;
  color: #fff;
  cursor: pointer;
  background: #000;
  width: 6rem;
  height: 6rem;
  z-index: 99;
}
.header-hum-menu span {
  font-weight: 500;
  display: block;
  width: 100%;
  margin-top: auto;
  margin-bottom: 0.3rem;
  opacity: 1;
  font-size: 0.9rem;
  font-family: "Lato";
}
button {
  background: none;
  border: none;
  padding: 0;
  font: 0 0 none;
}

.header-hum-menu i::before,
.header-hum-menu i::after {
  position: absolute;
  display: block;
  width: 100%;
  height: 1px;
  content: "";
  background: #fff;
}
.tel-group-content dt {
  padding-bottom: 0.3rem;
  margin-right: 1rem;
  border-bottom: 1px solid #fff;
  font-size: 1.3rem;
  letter-spacing: 3px;
}
.tel-group-content dd {
  font-weight: 500;
  margin-left: 0;
  font-size: 2.4rem;
}

.header-contact a {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 20rem;
  height: 4.8rem;
  border: 1px solid #fff;
  font-size: 1.4rem;
}

a {
  color: inherit;
  text-decoration: none;
  outline: 0;
}
.tel-group-open {
  font-size: 1.1rem;
  letter-spacing: 0.2px;
}
.header-hum-menu i::before {
  top: 100%;
}
/*    メニュー    */
.menu {
  position: fixed;
  z-index: 100;
  inset: 0;
  color: #fff;
  background: #222;
  padding: 2rem 2rem 0;
}
.menu-header {
  display: flex;
  justify-content: space-between;
}
.title-in-menu {
  font-size: 1.5rem;
  width: 18.8rem;
  color: #fff;
}
.close {
  position: relative;
  width: 45px;
  height: 6rem;
}
.close i::before {
  color: #fff;
  background: #fff;
  position: absolute;
  z-index: 1001;
  bottom: 0;
  transform: rotate(45deg);
  content: "";
  display: block;
  height: 1px;
  width: 6rem;
}
.close i::after {
  color: #fff;
  background: #fff;
  position: absolute;
  top: 0;
  transform: rotate(-45deg);
  content: "";
  display: block;
  height: 1px;
  width: 6rem;
}
.mail-contact {
  border-top: 1px solid rgba(255, 255, 255, 0.2);
  margin: 0 auto;
  text-align: center;
}
.menu-contact a {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 20rem;
  height: 4.8rem;
  border: 1px solid #fff;
  font-size: 1.4rem;
}
.tel-contact {
  border-top: 1px solid rgba(255, 255, 255, 0.2);
  margin: 0 auto;
  text-align: center;
}
@media screen and (min-width: 768px) {
  .header_tel-icon {
    display: none;
  }
  .header_tel-group {
    display: block;
    margin-right: 3rem;
  }

  .header-contact {
    display: block;
  }
  .header-content {
    height: 0;
    background: transparent;
    padding: 30px 0 30px 0;
    position: absolute;
    top: 8rem;
    left: 0;
    min-width: 108rem;
    transform: translate(0, -100%);
    width: 100%;
    align-items: center;
  }

  .header-content,
  .header-contents {
    color: #fff;
  }
  .header-title {
    font-size: 2.2rem;
    letter-spacing: 1px;
    padding-left: 5rem;
    width: 23rem;
  }

  .header-hum-menu {
    background: transparent;
    font-size: 1.1rem;
    width: 10rem;
    height: 10rem;
  }
  .header-hum-menu span {
    font-size: 1.1rem;
    margin-bottom: 0.6rem;
  }

  .header-hum-menu i {
    width: 3.5rem;
  }
  .header_email-icon {
    display: none;
  }
}
</style>

<script lang="ts">
import { Vue, Component } from "nuxt-property-decorator";

@Component({})
export default class extends Vue {
  isOpened = false;

  menuList = [
    "ALOについて",
    "ALOの強み",
    "ALOの商品紹介",
    "ご加盟までの流れ",
    "よくあるご質問"
  ];

  openMenu() {
    this.isOpened = !this.isOpened;
  }
}
</script>
