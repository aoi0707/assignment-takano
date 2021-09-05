<template>
  <section class="contact-group">
    <div class="contact section-inner">
      <h2 class="contact-text">お電話でのお問い合わせはこちら</h2>
      <div class="contact-tel">
        <div class="contact-tel-icon">
          <img src="contact-img.png" alt="contact-img" />
        </div>
        <dl class="contact-tel-number">
          <dt>0120-00-0000</dt>
          <dd>10:00〜18:00&nbsp;土日・祝日・年末年始除く</dd>
        </dl>
      </div>
    </div>
    <div class="contact-pagetop">
      <a class="scrollTo">
        <i class="scroll-icon">
          <img src="scroll-img.png" alt="scroll-icon" />
        </i>
        <p>PAGE&nbsp;TOP</p>
      </a>
    </div>
  </section>
</template>

<style scoped>
.contact-pagetop a {
  display: block;
}

a {
  color: inherit;
  text-decoration: none;
  outline: 0;
}

.scroll-icon {
  display: inline-block;
  font-style: normal;
  font-weight: normal;
  line-height: 1;
  -webkit-font-smoothing: antialiased;
}
.contact-pagetop {
  font-weight: 400;
  padding-bottom: 3.5rem;
  letter-spacing: 0.04em;
  font-size: 1.4rem;
}

.contact-tel-number dd {
  line-height: 1;
  margin: 0;
  font-size: 1rem;
}

.contact-tel-number dt {
  margin-bottom: 1rem;
  line-height: 1;
  font-size: 2.4rem;
}

.contact-tel-number {
  text-align: left;
  font-size: 0.875rem;
  margin: 0;
}

.contact-tel-icon {
  display: flex;
  align-items: center;
  margin-right: 1.2rem;
}

.contact-tel {
  display: flex;
  align-items: center;
  justify-content: center;
}

.contact-text {
  font-weight: 600;
  line-height: 1;
  font-size: 1.6rem;
  padding-bottom: 2rem;
  margin-bottom: 2rem;
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

h2 {
  margin: 0;
  font-size: 0;
  font-weight: 0;
}

.contact-group {
  color: #fff;
  text-align: center;
  background: #222;
  margin: 0 auto;
}

.contact {
  padding: 7rem 2rem;
}

@media only screen and (min-width: 768px) {
  .contact {
    text-align: center;
  }

  .contact-tel-icon {
    margin-right: 2rem;
  }

  .contact-tel-number dt {
    font-size: 3.6rem;
  }

  .contact-tel-number dd {
    font-size: 1.3rem;
    letter-spacing: 0.05rem;
  }
  .contact-text {
    font-weight: 600;
    line-height: 1;
    margin-bottom: 2.5rem;
    font-size: 1.6rem;
    padding: 0;
    border-bottom: 0;
  }
}
</style>

<script lang="ts">
import { Vue, Component } from "nuxt-property-decorator";

@Component({})
export default class extends Vue {}
</script>
