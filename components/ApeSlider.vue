<template>
    <div class="slider">
      <div class="image">
        <img src="~/assets/images/ape_slider.png" />
      </div>
      <div class="image">
        <img src="~/assets/images/ape_slider.png" />
      </div>
    </div>
</template>

<script>
export default {};
</script>

<style>
 
.slider {
 
  overflow: hidden;
  min-height: 35vh;
  height: 0vh;
  -webkit-mask-image: linear-gradient(
    transparent,
    black 20%,
    black 80%,
    transparent 100%
  );
}

.image {
  vertical-align: middle;
  animation: 12s linear 0s infinite normal none running loop;
}

.image:nth-child(1) {
  margin-top: 1px;
}

@keyframes loop {
  0% {
    transform: translateY(0px);
  }
  100% {
    transform: translateY(-100%);
  }
}
</style>
