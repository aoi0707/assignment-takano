<template>
  <section class="about_container">
    <!-- left -->
    <div class="about_inner ">
      <div class="about_left">
        <div class="about-left_inner">
          <h2 class="about-left_title">ABOUT</h2>
          <div class="about-left_alo">
            ABOUT&nbsp;ALO&nbsp;[&nbsp;ANIMAL&nbsp;LIBERATION&nbsp;ORCHESTRA&nbsp;]
          </div>
          <div class="about-left_dummy-txt-group dummy_txt-group">
            <div class="about-left_bg">
              <h3 class="about-left_dummy-txt-1">
                この文章はダミーです。<br />文字の大きさ、量、字間、行間等を確認するために<br />入れています。
              </h3>
              <div class="about-left_dummy-txt-2">
                <p>
                  この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。
                </p>
              </div>
            </div>
          </div>

          <div class="about-left_bg dummy_txt-group">
            <div class="about-left_dummy-txt-3 about_same-size-1">
              この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。
            </div>
            <div class="about-left_dummy-txt-4 about_same-size-2">
              <p>
                この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。
              </p>
            </div>
          </div>
        </div>
      </div>

      <!-- right -->
      <div class="about_right">
        <div class="about-right_img-1">
          <img src="about-img.png" alt="about-img" />
        </div>
        <div class="about-right_dummy-txt-group">
          <dl class="about-left_alo-animal-txt">
            <dt>ALO</dt>
            <dd>
              ANIMAL&nbsp;LIBERATION&nbsp;ORCHESTRA&nbsp;
            </dd>
          </dl>
          <div class="about-right_dummy-txt">
            この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。
          </div>
        </div>
        <div class="about-right_img-2">
          <img class="about-imgs" src="about-imgs.jpg" alt="about-imgs" />
        </div>
      </div>
    </div>

    <!-- number -->
    <div class="about_number">
      <div class=" about-number_inner section-inner">
        <div class="about-number_img-group">
          <div class="about-number_title">NUMBER&nbsp;OF<br />COMPLETIONS</div>
          <img src="number-of-completion-img.png" ait="number-img" />
        </div>
        <div class="about-number_dummy-txt-group">
          <div class="about-number_dummy-txt-1 about_same-size-1">
            この文章はダミーです。<br />文字の大きさ、量、字間を確認するため
          </div>
          <div class="about-number_dummy-txt-2">
            この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。この文章はダミーです。文字の大きさ、量、字間、行間等を確認するために入れています。
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
/* color */
.about_same-size-1,
.about-left_dummy-txt-1,
.about-left_alo {
  color: #45556a;
}

.about-number_dummy-txt-2 {
  line-height: 2;
  letter-spacing: 0.15rem;
  font-size: 1.6rem;
}
.about_number {
  padding: 7rem 2rem;
}
/* number */
.about-number_img-group {
  position: relative;
  margin-bottom: 4rem;
}
.about-number_title {
  color: rgba(34, 34, 34, 0.2);
  position: absolute;
  letter-spacing: 0;
  font-size: 3rem;
}
.about_same-size-2 {
  font-size: 1.6rem;
  letter-spacing: 0.01rem;
}

img {
  border-style: none;
  display: block;
  max-width: 100%;
  height: auto;
  margin: 0;
}
.about-left_alo-animal-txt dt {
  line-height: 1.25;
  font-size: 3.6rem;
}
.about-left_alo-animal-txt dd {
  line-height: 1.25;
  font-size: 1.2rem;
  margin: 1rem 0 0;
}
.about-left_alo-animal-txt::after {
  display: inline-block;
  width: 4rem;
  height: 1px;
  margin: 2.5rem 0 2.5rem;
  line-height: 1px;
  content: "";
  background: #fff;
}

/* left */
.about_container {
  padding: 7rem 0 0 0;
}
.about_same-size-1 {
  font-size: 2.4rem;
  margin-bottom: 3rem;
  line-height: 1.5;
  letter-spacing: 0.1rem;
}

.about-left_bg:nth-child(even) {
  background: #f5f5f5;
}
.about-left_dummy-txt-2 {
  font-size: 1.6rem;
  letter-spacing: 0.4px;
  line-height: 2;
}

.about-left_dummy-txt-1 {
  margin-bottom: 3rem;
  font-size: 2.4rem;
  line-height: 1.5;
  letter-spacing: 2px;
  letter-spacing: 0.2rem;
}

h3 {
  font-size: 0;
}

.about-left_alo {
  position: relative;
  line-height: 1.25;
  letter-spacing: 0.08em;
  font-size: 1.2rem;
  padding: 0 2rem;
  opacity: 50%;
  margin-bottom: 0;
}
.about-left_alo::before {
  position: absolute;
  top: 50%;
  display: block;
  width: 2rem;
  height: 1px;
  content: "";
  background: #45556a;
  transform: translate(calc(-100% - 1rem), -50%);
}

.about-left_title {
  margin-bottom: 1.2rem;
  font-size: 4.2rem;
  padding: 0 2rem;
}

h2 {
  font-size: 0;
  font-weight: 0;
}

.dummy_txt-group {
  padding: 4rem 2rem 7rem 2rem;
}

.about_right::before {
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
  display: block;
  width: 100%;
  height: 100%;
  content: "";
  background: #45556a;
}

.about_right {
  position: relative;
  color: #fff;
  /* width: 50%; */
}

.about-right_dummy-txt-group {
  padding: 0 2rem 5rem;
}

.about-right_img-1 {
  padding: 4rem 4rem 0;
}

.about-right_dummy-txt {
  margin-bottom: 3.5rem;
  font-size: 1.4rem;
}

@media screen and (min-width: 768px) {
  .about-imgs {
    margin-left: 20%;
  }

  .about_number {
    padding: 0;
  }
  .about_same-size-1 {
    letter-spacing: 0.2rem;
  }
  .about_container {
    padding: 0;
  }
  .about-left_alo {
    margin-bottom: 3.5rem;
    font-size: 1.2rem;
    padding: 0;
  }
  .about-left_alo::before {
    transform: translate(calc(-100% - 1.8rem), -50%);
  }
  .about-left_title {
    font-size: 6rem;
    padding: 0;
  }

  .about_inner {
    display: flex;
    padding: 0 4rem;
  }

  .about_left {
    width: 50%;
    padding-top: 14.5rem;
    display: flex;
    padding-bottom: 0;
  }

  .about-left_dummy-txt-1 {
    margin-bottom: 6rem;
    font-size: 3.2rem;
    line-height: 1.5;
    letter-spacing: 0.8rem;
  }
  .about-left_dummy-txt-2 {
    letter-spacing: 1.4px;
  }

  .about-left_bg:nth-child(even) {
    position: relative;
  }

  .about-left_bg > * {
    width: 85%;
  }
  .about_same-size-2 {
    line-height: 2;
    letter-spacing: 0.15rem;
  }
  .about-left_bg:nth-child(even)::after {
    position: absolute;
    top: 0;
    right: 0;
    z-index: -1;
    display: block;
    width: 50vw;
    height: 100%;
    content: "";
    background: #f5f5f5;
  }
  .about_right {
    position: relative;
    width: 50%;
  }
  .about_right::before {
    width: 50vw;
    overflow: hidden;
  }
  .about-right_dummy-txt-group {
    width: 70%;
    margin: -10rem 0 6rem auto;
    padding: 0;
  }

  .about-left_alo-animal-txt dt {
    margin-bottom: 3rem;
    font-size: 4.8rem;
  }

  .about-right_img-2 {
    position: absolute;
    max-width: 100%;
  }

  .about-number_inner {
    position: relative;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  .about-number_img-group {
    width: 50%;
    margin-bottom: 0;
  }
  .about-number_title {
    top: 2rem;
    line-height: 1.11111;
    font-size: 5.4rem;
  }
  .about-number_dummy-txt-group {
    width: 40%;
  }
}
</style>
