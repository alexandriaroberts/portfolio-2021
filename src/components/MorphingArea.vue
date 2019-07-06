<template>
  <div class="morphing-animation">
    <svg
      width="240"
      height="219"
      viewBox="0 0 240 219"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        d="M43 120C23 141 33.3741 141 21.5 141C9.62588 141 0 131.598 0 120C0 108.402 9.62588 99 21.5 99C33.3741 99 63 99 43 120Z"
        fill="#F23AA8"
      />
      <path
        d="M121.156 184.055C102.887 175.032 113.464 235.179 88.4632 214.732C63.4626 194.284 25 233.886 25 184.055C25 134.224 46.5253 92.0236 73.0782 92.0236C174.042 37.8869 121.156 134.224 121.156 184.055Z"
        fill="#F8E114"
      />
      <path
        d="M148.027 73.8998C160.164 82.5166 154.969 28.21 171.307 47.2747C187.645 66.3393 215.149 31.8626 213.488 76.608C211.826 121.353 195.765 158.641 177.689 157.893C107.15 203.661 146.366 118.645 148.027 73.8998Z"
        fill="#F86614"
      />
      <path
        d="M225.19 63.4729C206.256 58.1726 217.218 93.5037 191.308 81.4927C165.398 69.4817 125.537 92.7442 125.537 63.4729C125.537 34.2016 147.845 9.41248 175.364 9.41248C279.999 -22.3881 225.19 34.2016 225.19 63.4729Z"
        fill="#523AE2"
      />
    </svg>
  </div>
</template>

<script>
import { TimelineLite, TweenMax, Back } from "gsap";

export default {
  name: "MorphingArea",
  props: {
    msg: String
  },
  mounted() {}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
