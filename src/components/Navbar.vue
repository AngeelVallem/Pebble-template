<template>
  <div id="nav">
    <div class="logo-nav">
      <router-link to="/">
        <img class="img-logo" src="../assets/logo-p.png" alt="adoption-logo" />
      </router-link>
      <small class="name-logo">Adoption house</small>
    </div>
    <div class="flex_Item_Fill"></div>
    <div class="right-nav">
      <router-link class="nav-link" to="/about"> ADOPT NOW </router-link>
      <router-link class="nav-link" to="/about"> ABOUT US </router-link>
    </div>
  </div>  
</template>

<script>
export default {
name : 'Navbar'
}
</script>

<style lang="scss" scoped>
#nav {
   position: fixed;
  top: 0;
  width: 100%;
  display: flex;
  justify-content: space-between;
  padding: 10px 5rem;
  align-items: center;
  height: 6rem;
  background-color: #f6b8a9;
  box-shadow: 5px 1px 1px rgb(216, 211, 211);
  .logo-nav {
    display: flex;
    align-items: center;
    flex-direction: column;
  }
  .right-nav {
    .nav-link {
      margin-right: 50px;
      font-family: "Mate SC", serif;
      letter-spacing: 2px;
      text-decoration: none;
      font-weight: bold;
      color: #081b20;
      &:hover {
        text-decoration: underline;
        color: #081b20;
        transform: scale(1.1, 1.1);
      }
    }
  }
}

//Media queries
@media only screen and (max-width: 800px) {
  #nav {
    height: 5rem;
    padding: 3px 1px;
    .logo-nav {
      .img-logo {
        max-width: 120px;
      }
      .name-logo {
        display: none;
      }
    }
    .right-nav {
      .nav-link {
        color: #0e333c;
        margin-right: 1rem;
        font-size: 10px;
      }
    }
  }
}
</style>