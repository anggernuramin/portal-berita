<template>
  <Navbar />
  <!-- <Skeleton /> -->



  <div class="container">
    <form action="">
    <input type="text">
    <button type="submit">Search</button>
  </form>
    <section class="wrapper">
      <div class="box-wrapper-left">
        <div class="box">
          <div class="image-content">
            <img src="./assets/vue.svg" alt="logo" />
          </div>
          <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Labore, in
            nulla officiis vitae alias, velit perferendis fugiat suscipit
            corrupti culpa dicta omnis! Repellat nemo recusandae nulla quam vel,
            explicabo unde.
          </p>
        </div>
      </div>
      <div class="box-wrapper-right">
        <div class="box">
          <div class="image-content">
            <img src="./assets/vue.svg" alt="logo" />
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto
            praesentium quibusdam atque.
          </p>
        </div>
        <div class="box">
          <div class="image-content">
            <img src="./assets/vue.svg" alt="logo" />
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto
            praesentium quibusdam atque
          </p>
        </div>
        <div class="box">
          <div class="image-content">
            <img src="./assets/vue.svg" alt="logo" />
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto
            praesentium quibusdam atque
          </p>
        </div>
        <div class="box">
          <div class="image-content">
            <img src="./assets/vue.svg" alt="logo" />
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto
            praesentium quibusdam atque
          </p>
        </div>
      </div>
    </section>

    <section class="wrapper-reverse">
      <div class="box-wrapper-right">
        <div class="box">
          <div class="image-content">
            <img src="./assets/vue.svg" alt="logo" />
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto
            praesentium quibusdam atque
          </p>
        </div>
        <div class="box">
          <div class="image-content">
            <img src="./assets/vue.svg" alt="logo" />
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto
            praesentium quibusdam atque
          </p>
        </div>
        <div class="box">
          <div class="image-content">
            <img src="./assets/vue.svg" alt="logo" />
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto
            praesentium quibusdam atque
          </p>
        </div>
        <div class="box">
          <div class="image-content">
            <img src="./assets/vue.svg" alt="logo" />
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto
            praesentium quibusdam atque
          </p>
        </div>
      </div>
      <div class="box-wrapper-left">
        <div class="box">
          <div class="image-content">
            <img src="./assets/vue.svg" alt="logo" />
          </div>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto
            praesentium quibusdam atque
          </p>
        </div>
      </div>
    </section>
  </div>
</template>
<script >
import Navbar from "./components/Navbar.vue"
import Skeleton from "./components/Skeleton.vue"

export default {
  components: {
    Navbar,
    Skeleton
  }
};
</script>
<style scoped>


form{
 display: flex;
 justify-content: end;
 align-items: center;
 margin-bottom: 20px;
 gap: 10px;
}
form input {
font-size: 1rem;
  height: 30px;
  padding: 5px 10px;
  outline: none;
  border: 1px solid  #295D97;
  border-radius: 5px;
}
form button {
  font-size: 1rem;
  height: 30px;
  padding: 5px 10px;
  outline: none;
  border: 0;
  background-color:  #295D97;
  color: white;
  border-radius: 5px;
}


.box-wrapper-left {
  background-color: gainsboro;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: column;
  gap: 10px;
}
.image-content {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 60%;
  background-color: white;
  padding: 20px;
}
.image-content img {
  width: 100%;
  height: 100%;
  object-position: center;
  object-fit: contain;
}

.box-wrapper-left p {
  font-size: 1rem;
  padding: 20px;
}
.box-wrapper-right p {
  padding: 10px;
  font-size: 0.9rem;
}

.box-wrapper-right {
  display: grid;
  grid-template-columns: 49% 49%;
  grid-template-rows: 170px 170px;
  gap: 10px;
}

.box {
  border-radius: 5px;
  background-color: gainsboro;
  overflow: hidden;
  border: 1px solid rgba(0, 0, 0, 0.2);
}

@media only screen and (max-width: 600px) {
  .wrapper,
  .wrapper-reverse {
    grid-template-columns: 100%;
  }

  .wrapper-reverse .box-wrapper-left {
    grid-row-start: 1;
    grid-row-end: 1;
  }
  .container {
    width: 100%;
  }
}
</style>
