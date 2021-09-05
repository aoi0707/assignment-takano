<template>
  <footer>
    <div class="footer-inner">
      <div class="footer-text-group">
        <div class="footer-guide">企業案内</div>
        <div class="footer-p-policy">プライバシーポリシー</div>
      </div>
      <div class="footer-company">©︎&nbsp;COMPANY</div>
    </div>
  </footer>
</template>

<style scoped>
footer {
  background: #000000;
  color: #ffffff;
}
.footer-text-group {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  justify-content: center;
  padding: 3rem 0;
}

.footer-guide {
  font-size: 1.4rem;
  margin: 0.8rem 1rem;
}

.footer-p-policy {
  font-size: 1.4rem;
  margin: 0.8rem 1rem;
  line-height: 1;
}

.footer-company {
  display: flex;
  align-items: center;
  font-size: 1.4rem;
  justify-content: center;
  height: 7.6rem;
  text-align: center;
  border-top: 1px solid rgba(255, 255, 255, 0.2);
}

.footer-company {
  font-weight: 400;
}
.footer-inner {
  padding: 0 2rem;
}
@media only screen and (min-width: 768px) {
  .footer-inner {
    display: flex;
    align-items: center;
    justify-content: space-between;
    max-width: 128rem;
    height: 7rem;
    padding: 0 2.5rem;
    margin: 0 5rem;
    font-size: 0.875rem;
  }
  .footer-text-group {
    flex-wrap: nowrap;
    justify-content: none;
    padding: 0;
  }
  .footer-guide {
    margin: 0 4rem 0 0;
  }

  .footer-p-policy {
    margin: 0 4rem 0 0;
  }

  .footer-company {
    justify-content: none;
    height: 0;
    text-align: none;
    border-top: 0;
  }
}
</style>
