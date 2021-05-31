<template>
    <button :style="{ background: color, margin: m , color : textColor}">{{ text }}</button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String,
    color: String,
    m: {
      type: String,
      default: "1rem",
    },
    textColor : {
        type: String,
        default: '#000'
    }
  },
};
</script>

<style lang="scss" scoped>
button {
  display: inline-block;
  border: none;
  padding: 10px 30px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: 'Nunito', sans-serif;
  font-size: large;
  padding: 1rem;

  &:focus {
    outline: none;
  }
  &:active {
    transform: scale(0.98);
  }
}
</style>>

