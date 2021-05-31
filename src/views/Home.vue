<template>
  <div class="home">
    <section class="info-home">
      <div class="info">
        <h1>Find your new best friend</h1>
        <Button
        text='ADOPT NOW'
        color='#f6b8a9'
        textColor='#0F333C'
        m='1rem auto'
        />
      </div>
    </section>
    <section style="height:500px; margin-bottom: 3rem"></section>
  </div>
</template>

<script>
// @ is an alias to /src
import Button from '../components/Button'
export default {
  name: 'Home',
  components: {
    Button
  }
}
</script>


<style lang="scss" scoped>
  .home{
    margin: 4.5rem 0;

    .info-home{
      display: flex;
      height: 80vh;
      background-image: url('../assets/home-cover.png');
       background-size: cover;
      background-repeat: no-repeat;
      .info{
          h1{
            font-family: "Mate SC", serif;
            font-size: 3rem;
            color: #0F333C;
          }
          margin: 5rem auto;
          display: flex;
          flex-direction: column;        
      }
    }
  }
</style>
