<template>
  <div class="roadmapgoal">
    <div class="circular">
      <div class="inner"></div>
      <div class="number">{{ percentage }}%</div>
      <div class="circle">
        <div :class="'bar left p' + percentage">
          <div class="progress"></div>
        </div>
        <div :class="'bar right p' + percentage">
          <div class="progress"></div>
        </div>
      </div>
    </div>
    <p>
      {{ goal }}
    </p>
  </div>
</template>

<script>
export default {
  props: {
    percentage: Number,
    goal: String,
  },
};
</script>

<style>
.roadmap {
  width: 60%;
  margin: auto;
  display: grid;
  row-gap: 1rem;
}

.roadmapgoal {
  display: grid;
  grid-template-columns: 10rem 3fr;
  align-items: center;
}

.roadmapgoal p {
  color: white;
  font: 18px "Arial";
  text-align: center;
}

.circular {
  height: 100px;
  width: 100px;
  position: relative;
  transform: scale(1);
}

.circular .inner {
  position: absolute;
  z-index: 6;
  top: 50%;
  left: 50%;
  height: 80px;
  width: 80px;
  margin: -40px 0 0 -40px;
  background: #fff;
  border-radius: 100%;
}

.circular .number {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: 10;
  font: 24px HighSchool;
  color: #10150b;
}

.circular .bar {
  position: absolute;
  height: 100%;
  width: 100%;
  background: #fff;
  -webkit-border-radius: 100%;
  clip: rect(0px, 100px, 100px, 50px);
}

.circle .bar .progress {
  position: absolute;
  height: 100%;
  width: 100%;
  -webkit-border-radius: 100%;
  clip: rect(0px, 50px, 100px, 0px);
  background: #10150b;
}

.circle .left .progress {
  z-index: 1;
  animation: left 2s linear both;
}

.circle .right {
  transform: rotate(180deg);
  z-index: 3;
}

.circle .right .progress {
  animation: right 2s linear both;
  animation-delay: 2s;
}

.p10 {
  --l: rotate(36deg);
}

.p20 {
  --l: rotate(72deg);
}

.p40 {
  --l: rotate(144deg);
}

.p60 {
  --l: rotate(180deg);
  --r: rotate(36deg);
}

.p80 {
  --l: rotate(180deg);
  --r: rotate(108deg);
}

.p100 {
  --l: rotate(180deg);
  --r: rotate(180deg);
}

@keyframes right {
  100% {
    transform: var(--r);
  }
}

@keyframes left {
  100% {
    transform: var(--l);
  }
}
</style>
