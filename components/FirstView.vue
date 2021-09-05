<template>
  <div class="main-content">
    <div class="img-content">
      <img src="/first-img.jpg" alt="FirstView" />
    </div>
    <div class="first-text-area">
      <div class="first-inner-area">
        <div class="text-ja-alo">日本ALO音楽研究所</div>
        <div class="first-text">
          <img
            src="/first-text-ALO.png"
            alt="ALO ANIMAL LIBERATION ORCHESTRA"
          />
        </div>

        <h2>この文章はダミーです。</h2>
        <div class="text-animal">ANIMAL&nbsp;LIBERATION&nbsp;ORCHESTRA</div>
        <p>
          この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.main-content {
  background: #222222;
  position: relative;
  margin-top: 60px;
  height: calc(100vh - 60px);
  width: 100%;
}

.first-text-area {
  color: #ffffff;
  position: absolute;
  z-index: 1;
  max-width: 64rem;
  margin-top: -3.5rem;
}

/* ----------------------------------------- */
.first-inner-area {
  padding: 0 3rem 6rem;
}
.first-inner-area p {
  font-size: 1.4rem;
}
.first-text {
  margin-bottom: 3.5rem;
}

.first-inner-area h2 {
  margin-bottom: 2rem;
  font-size: 2.5rem;
}
.text-animal {
  margin-bottom: 3rem;
  letter-spacing: 2px;
  font-size: 1.2rem;
}
.text-ja-alo {
  display: none;
  margin-bottom: 3rem;
  letter-spacing: 3px;
  font-size: 2.6rem;
}
.img-content {
  width: 100%;
  position: relative;
  overflow: hidden;
}

img {
  display: block;
  width: 110%;
}
@media screen and (min-width: 768px) {
  .img-content {
    width: 69.44444%;
  }
  .main-content {
    width: 100%;
    margin: 0;
    height: auto;
  }
  .img-content::before {
    position: absolute;
    display: block;
    width: 28%;
    right: 0;
    /* z-index: 1; */
    height: 100%;
    background: rgba(0, 0, 0, 0.5);
    content: "";
    animation: fadeIn 0.5s ease 0s 1 normal backwards;
  }
  @keyframes fadeIn {
    from {
      opacity: 0;
      width: 0%;
      /* transform: translateX(50%); */
    }
    to {
      opacity: 1;
      width: 28%;
      /* transform: translateX(0); */
    }
  }
  .first-text-area {
    top: 50%;
    left: 50%;
    width: 50%;
    transform: translate(0, -50%);
  }
  .first-inner-area {
    width: 86.66667%;
    margin-right: 0;
    margin-left: auto;
    padding: 0;
  }
  .first-inner-area h2 {
    margin-bottom: 1rem;
    font-size: 3.8rem;
  }
  .text-animal {
    margin-bottom: 5rem;
    letter-spacing: 3px;
    font-size: 1.8rem;
  }
  .text-ja-alo {
    display: block;
  }
  .first-inner-area p {
    font-size: 1.6rem;
  }
  .first-text {
    max-width: 90%;
    margin-bottom: 10rem;
  }
}
</style>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({});
</script>
