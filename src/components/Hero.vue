<template>
  <div
    class="flex mt-24 h-screen-80 max-w-7xl m-center md:flex-col lg:flex-row md:pt-10"
    id="home"
  >
    <div class="flex flex-col items-start m-auto info lg:w-3/6">
      <h2
        data-aos="fade-right"
        data-aos-delay="500"
        data-aos-duration="500"
        class="pb-3 text-5xl font-extrabold duration-1000 f-black name dark:text-white"
      >
        Bernard Andrew <br> De Guzman
      </h2>
      <h4
        class="pb-2 text-lg duration-1000 f-gray dark:text-white"
        data-aos="fade-right"
        data-aos-delay="700"
        data-aos-duration="500"
      >
        Software Engineer
      </h4>
      <h5
        class="pb-12 text-sm duration-1000 f-gray dark:text-white"
        data-aos="fade-right"
        data-aos-delay="800"
        data-aos-duration="500"
      >
        I am an experienced full stack engineer, worked on several projects ranging from e-commerce, blogs, forum and api integrations. I'm also an Information Technology Student at Polytehnic University of the Philippines
      </h5>
      <div data-aos="fade-right" data-aos-delay="800" data-aos-duration="700">
        <a
          class="flex items-center cursor-pointer btn-accent"
          href="mailto:deguzmanbernardandrew@gmail.com"
        >
          <span> Contact Me&nbsp;</span>
          <span
            ><font-awesome-icon class="w-4" :icon="['fas', 'paper-plane']"
          /></span>
        </a>
      </div>
    </div>
    <div class="flex hidden profile-image lg:w-3/6 md:flex md:m-auto md:pt-16">
      <img
        data-aos="zoom-in-right"
        data-aos-delay="1500"
        data-aos-duration="800"
        :class="`m-auto clipped light ismall img-first md:w-auto`"
        src="https://drive.google.com/thumbnail?sz=w1920&id=1SNQz-GgCvN3ZNLoe3ucBlawldui8QrYn"
        alt=""
        width="400"
      />
      <img
        data-aos="zoom-in-right"
        data-aos-delay="1700"
        data-aos-duration="800"
        class="m-auto clipped light imedium img-center md:w-auto"
        src="https://drive.google.com/thumbnail?sz=w1920&id=1q1b-K77wHYC9tW60LU5v2Wno-KZzXk0w"
        alt=""
        width="400"
      />
      <img
        data-aos="zoom-in-right"
        data-aos-delay="1900"
        data-aos-duration="800"
        class="m-auto clipped light ismall img-last md:w-auto"
        src="https://drive.google.com/thumbnail?sz=w1920&id=1QI518PJIDWIVO4DNlroajnFOm306aVJf"
        alt=""
        width="400"
      />
    </div>
  </div>
</template>
<script lang="ts" setup>
import { watch } from "@vue/runtime-dom";
import { useDark, useToggle } from "@vueuse/core";
const isDark = useDark();
</script>
<style lang="scss" scoped>
.clipped {
  clip-path: polygon(25% 0%, 100% 0%, 75% 100%, 0% 100%);
}
.ismall {
  height: 19rem;
}
.imedium {
  height: 25rem;
}

.img-first {
  margin-left: 12px;
  height: 350px;
  clip-path: polygon(25% 0%, 100.5% 0%, 73% 100%, 0% 100%);
}

.img-center {
  margin-left: -66px;
}

.img-last {
  margin-left: -65px;
}

.light {
  filter: grayscale(40%);
  transition: 0.5s ease-out 100ms;
  cursor: pointer;

  &:hover {
    filter: grayscale(0);
    transform: scale(1.03);
    z-index: 999;
  }

  &.colored {
    filter: grayscale(0) !important;
  }
}

.profile-image {
  &::after {
    content: "";
    position: absolute;
    bottom: 120px;
    background: rgba(80, 80, 80, 0.503);
    width: 25rem;
    height: 50px;
    border-radius: 50%;
    filter: blur(20px);
    margin-left: 6rem;
  }
}
</style>
