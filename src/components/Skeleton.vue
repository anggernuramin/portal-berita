<template>
  <div class="container">
    <section class="wrapper">
      <div class="box-wrapper-left">
        <div class="box"></div>
      </div>
      <div class="box-wrapper-right">
        <div class="box"></div>
        <div class="box"></div>
        <div class="box"></div>
        <div class="box"></div>
      </div>
    </section>

    <section class="wrapper-reverse">
      <div class="box-wrapper-right">
        <div class="box"></div>
        <div class="box"></div>
        <div class="box"></div>
        <div class="box"></div>
      </div>
      <div class="box-wrapper-left">
        <div class="box"></div>
      </div>
    </section>
  </div>
</template>

<style >


.box-wrapper-left {
  background: linear-gradient(90deg, #f0f0f0 25%, #e0e0e0 50%, #f0f0f0 75%);
  background-size: 400% 100%;
  animation: shimmer 1.5s infinite linear;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: column;
  gap: 10px;
}

.box-wrapper-right {
  display: grid;
  grid-template-columns: 49% 49%;
  grid-template-rows: 170px 170px;
  gap: 10px;
}

.box-wrapper-left .box, .box-wrapper-right .box {
  border-radius: 5px;
  background: linear-gradient(90deg, #f0f0f0 25%, #e0e0e0 50%, #f0f0f0 75%);
  background-size: 400% 100%;
  animation: shimmer 1.5s infinite linear;
}

@keyframes shimmer {
  0% {
    background-position: 0 0;
  }
  100% {
    background-position: 100% 0;
  }
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

<!-- <template>
  <div class="skeleton-loading">
    <div class="skeleton-wrapper">
      <div class="skeleton"></div>
    </div>
    <div class="skeleton-text">
      <div class="skeleton skeleton-long"></div>
      <div class="skeleton skeleton-short"></div>
      <div class="skeleton skeleton-medium"></div>
    </div>
  </div>
</template> -->

