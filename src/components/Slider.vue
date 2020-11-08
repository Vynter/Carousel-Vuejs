<template>
  <div>
    <div class="mainSlide">
      <font-awesome-icon
        class="left icon"
        :icon="['fas', 'arrow-circle-left']"
        on:click="moveLeft"
      />
      <div style="" class="slidecontainer">
        <!-- <img src="../assets/1-800x600.jpg" alt="" />
        <img src="../assets/2-800x600.jpg" alt="" />
        <img src="../assets/3-800x600.jpg" alt="" />
        <img src="../assets/4-800x600.jpg" alt="" /> -->
        <img src="../assets/1-800x600.jpg" alt="" />
        <img src="../assets/2-800x600.jpg" alt="" />
        <img src="../assets/3-800x600.jpg" alt="" />
        <img src="../assets/4-800x600.jpg" alt="" />
      </div>

      <font-awesome-icon
        class="right icon"
        :icon="['fas', 'arrow-circle-right']"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "Slider",
  data() {
    return {
      pos: 0,
    };
  },
  methods: {
    moveLeft: function() {},
  },
};
</script>

<style scoped>
.mainSlide {
  position: relative;
  width: 900px;
  margin: auto;
  border: 1px solid red;
  overflow: hidden;
}
.slidecontainer {
  width: 800px;
  height: 600px;
  margin: auto;
  border: 1px solid blue;
  display: flex;
  transition: 1s;
  transform: translateX(-2400px);
}
.left,
.right {
  text-decoration: none;
  /*display: inline-block;*/
  position: absolute;
  top: 50%;
  color: black;
  z-index: 5;
}
.left {
  left: 0%;
}
.right {
  right: 0%;
}
.icon {
  font-size: 38px;
}
</style>
