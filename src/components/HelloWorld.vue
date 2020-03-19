<template>
  <div class="hello">
    <div class="pimg1 vh-100">
      <div class="ptext">
        <span class="border">My Website</span>
      </div>
    </div>
    <section class="section section-light">
      <h1>{{ msg }}</h1>
      <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Pariatur quos illum in molestiae harum recusandae aliquam, iste aut facere dolore?</p>
    </section>

    <div class="pimg2">
      <div class="ptext">
        <span class="border trans">Image Two Text</span>
      </div>
    </div>
    <section class="section section-dark">
      <h1>{{ msg }}</h1>
      <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Pariatur quos illum in molestiae harum recusandae aliquam, iste aut facere dolore?</p>
    </section>

    <div class="pimg3">
      <div class="ptext">
        <span class="border trans">Image Three Text</span>
      </div>
    </div>
    <section class="section section-dark">
      <h1>{{ msg }}</h1>
      <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Pariatur quos illum in molestiae harum recusandae aliquam, iste aut facere dolore?</p>
    </section>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
body,
html {
  height: 100%;
  margin: 0;
  font-size: 16px;
  font-family: "Lato", sans-serif;
  font-weight: 400;
  line-height: 1.8em;
  color: #666;
}

.pimg1,
.pimg2,
.pimg3 {
  position: relative;
  opacity: 0.7;
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;

  /*
    fixed = parallax
    scroll = normal
  */
  background-attachment: fixed;
}

.pimg1 {
  background-image: url("../assets/img/image1.jpg");
  min-height: 400px;
}

.pimg2 {
  background-image: url("../assets/img/image2.jpg");
  min-height: 400px;
}

.pimg3 {
  background-image: url("../assets/img/image3.jpg");
  min-height: 400px;
}

.section {
  text-align: center;
  padding: 50px 80px;
}

.section-light {
  background-color: #f4f4f4;
  color: #666;
}

.section-dark {
  background-color: #282e34;
  color: #ddd;
}

.ptext {
  position: absolute;
  top: 50%;
  width: 100%;
  text-align: center;
  color: #000;
  font-size: 27px;
  letter-spacing: 8px;
  text-transform: uppercase;
}

.ptext .border {
  background-color: #111;
  color: #fff;
  padding: 20px;
}

.ptext .border.trans {
  background-color: transparent;
}

@media (max-width: 568px) {
  .pimg1,
  .pimg2,
  .pimg3 {
    background-attachment: scroll;
  }
}
</style>
