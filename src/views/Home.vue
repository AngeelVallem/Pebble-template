<template>
  <div class="home">
    <section class="info-home">
      <div class="info">
        <h1>Find your new best friend</h1>
        <router-link 
        to="/adopt"
        class="homeb"
        >
          <Button
          text="ADOPT NOW"
          color="#f6b8a9"
          textColor="#0F333C"
        />
        </router-link>
      </div>
    </section>
    <section class="seenin">
      <p>As Seen in</p>
      <ul>
        <li><img src="../assets/today-logo.jpg" alt="today logo" /></li>
        <li><img src="../assets/GMA-logo.jpg" alt="today logo" /></li>
        <li><img src="../assets/NBC-logo.png" alt="today logo" /></li>
      </ul>
    </section>
    <img class="dot-layer" src="../assets/Layer_5_4.png" alt="layer1" />
    <section class="Section">
      <img class="hug" src="../assets/hug_1_800x.png" alt="hug" />
      <div class="Section-header">
        <h3>Human-Grade Care Your Pets Deserve</h3>
      </div>
      <div class="blue-content">
        <div class="blue">
          <img src="../assets/thumbsup03.png" alt="thumbssup" />
          <h4>HUMA-GRADE QUALITY</h4>
          <p>
            We use human-grade ingredients & FDA-inspected facilities. All our
            products are third-party tested for purity & potency.
          </p>
        </div>
        <div class="blue">
          <img src="../assets/Name_priceTAG_1_800x.png" alt="bone" />
          <h4>FAIR RICING</h4>
          <p>
            We kicked out the middleman and put you and your pet at the center.
            No retail mark-ups, no marketing gimmicks.
          </p>
        </div>
        <div class="blue">
          <img src="../assets/award_1_800x.png" alt="award" />
          <h4>TRANSPARENCY</h4>
          <p>
            We share where our ingredients come from, and where we manufacture
            our products.
          </p>
        </div>
      </div>
    </section>
    <section class="mission">
      <img src="../assets/idea_1_800x.png" alt="idea" />
      <h3>OUR MISSION</h3>
      <h2>Helping Senior Shelter Dogs</h2>
      <div class="mission-p">
        <p>
          Our mission is to help senior shelter dogs, and for every product
          purchased, we donate one to shelters that give senior dogs a second
          chance in life.
        </p>
        <p>
          We offer the same formulas as major brand names at wallet-friendly
          prices. No middleman. No upcharge.
        </p>
        <p>Just exceptional care that won’t break the bank!</p>
      </div>
    </section>
    <img class="dot-layer2" src="../assets/dot-layer2.png" alt="d2">
    <div style="height: 300px; margin: 1rem 0"></div>
  </div>
</template>

<script>
// @ is an alias to /src
import Button from "../components/Button";
export default {
  name: "Home",
  components: {
    Button,
  },
};
</script>


<style lang="scss" scoped>
.home {
  margin: 4.5rem 0;

  .info-home {
    display: flex;
    height: 80vh;
    background-image: url("../assets/home-cover.png");
    background-size: cover;
    background-repeat: no-repeat;
    .info {
      h1 {
        font-family: "Mate SC", serif;
        color: #0f333c;
      }
      margin: 5rem auto;
      display: flex;
      flex-direction: column;
      .homeb{
        display: flex;
        justify-content: center;
        text-decoration: none;
      }
    }
  }
  .seenin {
    p {
      text-align: center;
      margin: 2rem 0;
      font-family: "Nunito", sans-serif;
      font-size: 1.5rem;
      font-weight: bold;
    }

    ul {
      margin: 0;
      padding: 0;
      list-style-position: inside;
      margin-top: 0;
      margin-bottom: 10px;
      text-align: center;
      li {
        max-width: 125px;
        display: inline-block;
        margin: 0 120px 35px;
        text-align: center;
        img {
          width: 100%;
          vertical-align: middle;
        }
      }
    }
  }

  .dot-layer {
    display: none;
  }
  .Section {
    background-color: #fbece9;
    padding: 30px;
    margin-top: 300px !important;
    .hug {
      display: none;
    }

    h3 {
      font-family: "Mate SC", serif;
      max-width: 423px;
      color: #0f333c;
      font-size: 2.5rem;
      letter-spacing: 2px;
    }

    .blue {
      margin: 2rem 0;

      h4 {
        font-family: "Mate SC", serif;
        font-size: 1.5rem;
        margin-bottom: 2rem;
      }
      p {
        font-family: "Nunito", sans-serif;
        font-size: 1.1rem;
      }
    }
  }
  .mission {
    display: flex;
    align-items: center;
    flex-direction: column;
    padding: 2rem;
    img {
      max-width: 200px;
    }

    h3 {
      font-family: "Nunito", sans-serif;
      font-size: 1.5rem;
      font-weight: 900;
      margin: 0.8rem 0;
    }
    h2 {
      text-align: center;
      font-family: "Mate SC", serif;
      color: #0f333c;
      font-size: 2.5rem;
      margin-bottom: 1.5rem;
    }
    .mission-p {
      text-align: center;
      max-width: 60%;
      p {
        font-family: "Nunito", sans-serif;
        font-size: 1.5rem;
        font-weight: bolder;
        margin-bottom: 1.5rem;
      }
    }
  }
}

@media only screen and (min-width: 768px) {
  .info {
    h1 {
      font-size: 3rem;
    }
  }
  .seenin {
    margin-bottom: 5rem;
  }
  .Section {
    .Section-header {
      text-align: center;
      h3 {
        margin-top: 80px;
        margin: 0 auto !important;
      }
    }

    .blue {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;

      img {
        max-width: 250px;
      }
      p {
        text-align: center;
        width: 50%;
      }
    }
  }
}
@media only screen and (min-width: 1024px) {
  .dot-layer {
    display: block !important;
    position: absolute;
    margin-top: -100px;
    width: 20%;
  }

  .Section {
    margin: 0 70px;
    margin-top: 200px;
    margin-bottom: 100px;
    padding: 80px 70px !important;

    .hug {
      display: block !important;
      position: absolute;
      margin-top: -300px;
      right: 0px;
      width: 45%;
    }

    .Section-header {
      display: flex;
      width: 40%;
      justify-content: start;

      h3 {
        text-align: start;
        margin-top: 80px;
        margin: 0;
      }
    }

    .blue-content {
      display: flex;
    }
  }
}
</style>
