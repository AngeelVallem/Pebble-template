<template>
  <div class="footer-top"></div>
  <footer class="Footer">
    <div class="newsletter">
      <div class="form">
        <h1>Subscribe for pets tips</h1>
        <input type="email" name="email" class="newsletter-input" />
        <Button
          text="SUBSCRIBE"
          color="#0E333C"
          textColor="#C0CCFC"
          m="1rem 0"
        />
      </div>
      <img src="../assets/sittingdog_3.png" alt="" />
    </div>
    <div class="footer-container">
      <div class="footer-heading">
        <router-link to="/">
          <img src="../assets/logo-pp.png" alt="logoPP" />
        </router-link>
        <ul>
          <li><a href="#">CONTACT US</a></li>
          <li><a href="#">TERMS</a></li>
          <li><a href="#">PRIVACY</a></li>
        </ul>
      </div>
      <div class="footer-secondary">
        <ul>
          <li><router-link to="/">FIND A DOG</router-link></li>
          <li><router-link to="/">FIND A CAT</router-link></li>
          <li><router-link to="/">ADOPTED PETS</router-link></li>
        </ul>
      </div>
      <div class="footer-utilities">
        <router-link to="/adopt">
          <Button m="2rem 1rem" text="ADOPT NOW" color="#f3a490" />
        </router-link>
        <div>
          <a href="#">
            <img src="../assets/facebook-pp.svg" alt="" />
          </a>
          <a href="#">
            <img src="../assets/twitter-pp.svg" alt="" />
          </a>
          <a href="#">
            <img src="../assets/instagram-pp.svg" alt="" />
          </a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import Button from "./Button";

export default {
  name: "Footer",
  components: {
    Button,
  },
};
</script>

<style lang="scss" scoped>
.footer-top {
  display: none;
  background-image: url("../assets/footer-top.png");
  background-size: cover;
  background-repeat: no-repeat;
  position: relative;
  top: 50px;
  height: 135px;
}
.Footer {
  background-color: #0e333c;
  .newsletter {
    max-width: 980px;
    height: 278px;
    background: #c0ccfc;
    margin: 0px auto;
    position: relative;
    top: -245px;

    display: flex;
    justify-content: center;
    align-items: center;
    .form {
      max-width: 80%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: start;

      h1 {
        font-size: 25px;
        font-family: Apercu Pro;
      }
      .newsletter-input {
        appearance: none;
        width: 250px;
        margin: 1rem 0;
        border: 1px solid #dbe0e2;
        border: none;
        padding: 12px 14px;
        color: #0E333C;
        background: #fff;
        font-family: Apercu Pro;
        font-style: normal;
        font-weight: 500;
        font-size: 18px;
        line-height: 28px;
        resize: none;

        &:focus-visible{
          outline: 2px solid #0E333C;
        }
      }
    }

    img {
      z-index: 1;
      display: none;
      max-width: 100%;
      height: auto;
      border-style: none;
      vertical-align: top;
      position: absolute;
      right: 0px;
      top: -114px;
    }
  }
  .footer-container {
    display: flex;
    flex-direction: column;
    padding-bottom: 4rem;
    padding: 0rem 4rem  ;
    .footer-heading {
      display: flex;
      flex-direction: column;
      ul {
        list-style: none;
        margin: 1rem 0;
        li {
          margin: 0.5rem 0;
          a {
            text-decoration: none;
            color: #f6b8a9 !important;
            &:hover {
              font-weight: bold;
            }
          }
        }
      }
    }
    .footer-secondary {
      ul {
        list-style: none;
        li {
          margin: 0.5rem 0;
          a {
            text-decoration: none;
            color: #f6b8a9;

            &:hover {
              font-weight: bold;
            }
          }
        }
      }
    }
    .footer-utilities {
      margin: 2rem 0;
      a {
        margin-right: 2rem;
      }
    }
  }
}

@media only screen and (min-width: 768px) {
  .footer-top {
    display: block;
  }
  .Footer {
    .newsletter {
      display: block;
      padding-left: 55px;
      padding-top: 44px;
      height: 262px;
      img {
        display: block;
      }
    }
    .footer-container {
      flex-direction: row;
      justify-content: space-between;
      align-items: center;
      padding: 0rem 4rem;
      font-size: 1.5rem;
    }
  }
}
</style>