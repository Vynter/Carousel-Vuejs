<template>
  <div>
    <div class="mainSlide">
      <a class="left" href="">
        <font-awesome-icon class="icon" :icon="['fas', 'arrow-circle-left']"
      /></a>
      <div class="slidecontainer">
        <img src="../assets/1 800x600.jpg" alt="" />
        <img src="../assets/2 800x600.jpg" alt="" />
        <img src="../assets/3 800x600.jpg" alt="" />
        <img src="../assets/4 800x600.jpg" alt="" />
      </div>
      <a class="right" href="">
        <font-awesome-icon class="icon" :icon="['fas', 'arrow-circle-right']"
      /></a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Slider",
};
</script>

<style scoped>
.mainSlide {
  position: relative;

  border: 1px solid red;
}
.slidecontainer {
  width: 800px;
  height: 600px;
  margin: auto;
  border: 1px solid blue;
}
.left,
.right {
  text-decoration: none;
  display: inline-block;
  position: absolute;
  top: 50%;
  color: black;
}
.left {
  left: 10%;
}
.right {
  right: 10%;
}
.icon {
  font-size: 38px;
}
</style>
