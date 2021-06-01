<template>
  <div>
      <h1>1</h1>
      <h1>2</h1>
      <h1>3</h1>
      <h1>4</h1>
       <h1>1</h1>
    <h1>2</h1>
    <h1>3</h1>
    <h1>4</h1>
    <h1>9</h1>
    <h1>10</h1>
    <h1>11</h1>
    <h1>12</h1>
    <h1>13</h1>
  </div>
</template>

<script>
export default {
name : 'Adopt',
methods: {

},
async mounted(){    

    const res = await fetch('https://www.petrescue.com.au/api/listings')
    const data = await res.json()

    console.log(data);
}
}
</script>

<style>

</style>