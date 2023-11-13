<template>
  <div class="max-w-7xl m-center pt-20" id="projects">
    <div
      class="about-me text-center mt-10 md:mt-32"
      data-aos="fade-up"
      data-aos-delay="100"
      data-aos-duration="800"
    >
      <h2 class="text-5xl dark:text-white">Portfolio</h2>
      <span class="f-gray text-sm dark:text-white">Recent Projects</span>
    </div>
    <div
      class="details flex gap-10 justify-center"
      data-aos="fade-left"
      data-aos-delay="500"
      data-aos-duration="600"
    >
      <swiper
        :slidesPerView="3"
        :spaceBetween="0"
        :centeredSlides="true"
        :pagination="{
          clickable: true,
        }"
        :modules="modules"
        :breakpoints="{
          '200': {
            slidesPerView: 1,
          },
          '600': {
            slidesPerView: 2,
            spaceBetween: 25,
          },
          '768': {
            slidesPerView: 3,
          },
        }"
        class="mySwiper"
      >
        <swiper-slide v-for="(project, key) in recent_projects" :key="key">
          <div
            class="custom-card bg-white dark:bg-slate-800 drop-shadow-2xl w-80 h-96 rounded"
          >
            <div class="tools">
              <div class="circle">
                <span class="red box"></span>
              </div>
              <div class="circle">
                <span class="yellow box"></span>
              </div>
              <div class="circle">
                <span class="green box"></span>
              </div>
            </div>
            <div class="card__content p-2 flex flex-col justify-between">
              <div class="flex flex-col gap-2">
                <div class="project-img">
                  <img
                    :src="project.project_logo"
                    alt=""
                    :class="`${project.class} thumbnail m-auto max-h-48 object-cover`"
                  />
                </div>
                <div class="title dark:text-white text-2xl font-semibold pt-2">
                  {{ project.name }}
                </div>
                <div class="description text-sm text-gray-400">
                  {{ project.description }}
                </div>
              </div>
              <div class="visit-link flex justify-center">
                <a
                  class="cssbuttons-io-button bg-cyan-500 w-44 cursor-pointer"
                  :href="project.project_link"
                  target="_blank"
                >
                  Visit Site
                  <div class="icon">
                    <svg
                      class="text-cyan-500"
                      height="24"
                      width="24"
                      viewBox="0 0 24 24"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path d="M0 0h24v24H0z" fill="none"></path>
                      <path
                        d="M16.172 11l-5.364-5.364 1.414-1.414L20 12l-7.778 7.778-1.414-1.414L16.172 13H4v-2z"
                        fill="currentColor"
                      ></path>
                    </svg>
                  </div>
                </a>
              </div>
            </div>
          </div>
        </swiper-slide>
      </swiper>
    </div>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";

import "swiper/css";

import "swiper/css/pagination";

// import required modules
import { Pagination } from "swiper";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },

  setup() {
    return {
      modules: [Pagination],
    };
  },

  data() {
    return {
      recent_projects: [
        {
          name: "Pili-Pinas",
          project_link: "https://pili-pinas.onrender.com/",
          project_logo: "https://drive.google.com/uc?id=16zcPBc_Ag6Nv-NTg39WNUSHF_tdBNW7I",
          description: "Capstone Project Streamlining the travel experience",
          class: "pili-pinas",
        },
        {
          name: "Wordle Clone",
          project_link: "https://theadg.github.io/wordle-clone/",
          project_logo:
            "https://static01.nyt.com/images/2022/03/02/crosswords/alpha-wordle-icon-new/alpha-wordle-icon-new-square320-v3.png?format=pjpg&quality=75&auto=webp&disable=upscale",
          description: "Clone of the pandemic hit game",
          class: "wordle",
        },
        {
          name: "The Do List",
          project_link: "https://theadg.github.io/todo-list/",
          project_logo:
            "https://static-00.iconduck.com/assets.00/check-mark-button-emoji-2048x2048-lq7rf7h8.png",
          description: "Essential CRUD Project",
          class: "the do list",
        },

        {
          name: "Tic Tac Toe",
          project_link: "https://theadg.github.io/tic-tac-toe/",
          project_logo: "https://em-content.zobj.net/source/skype/289/o-button-blood-type_1f17e-fe0f.png",
          description:
            "A classic on the browser",
          class: "tic tac toe ",
        },
      ],
    };
  },
};
</script>

<style scoped>
.custom-card {
  border-radius: 8px;
  z-index: 1;
  height: 26rem;
}

.tools {
  display: flex;
  align-items: center;
  padding: 9px;
}

.circle {
  padding: 0 4px;
}

.box {
  display: inline-block;
  align-items: center;
  width: 10px;
  height: 10px;
  padding: 1px;
  border-radius: 50%;
}

.red {
  background-color: #ff605c;
}

.yellow {
  background-color: #ffbd44;
}

.green {
  background-color: #00ca4e;
}

.swiper {
  width: 100%;
  height: 65vh;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;

  /* Center slide text vertically */
  display: -webkit-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  -webkit-justify-content: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  -webkit-align-items: center;
  align-items: center;
}

.swiper-slide img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.capitan,
.vwala {
  clip-path: circle(30% at 50% 50%);
}

.cssbuttons-io-button {
  color: white;
  font-family: inherit;
  padding: 0.35em;
  padding-left: 1.2em;
  font-size: 17px;
  font-weight: 500;
  border-radius: 0.9em;
  border: none;
  letter-spacing: 0.05em;
  display: flex;
  align-items: center;
  overflow: hidden;
  position: relative;
  height: 2.8em;
  padding-right: 3.3em;
}

.cssbuttons-io-button .icon {
  background: white;
  margin-left: 1em;
  position: absolute;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 2.2em;
  width: 2.2em;
  border-radius: 0.7em;
  right: 0.3em;
  transition: all 0.3s;
}

.cssbuttons-io-button:hover .icon {
  width: calc(100% - 0.6em);
}

.dsg,
.fundspace {
  width: 90% !important;
}

.fundspace {
  padding-top: 3rem;
}

.richardson {
  padding-top: 2rem;
}

.bms {
  padding-top: 1rem;
}

.cmdi {
  width: 40% !important;
}

.cssbuttons-io-button .icon svg {
  width: 1.1em;
  transition: transform 0.3s;
}

.cssbuttons-io-button:hover .icon svg {
  transform: translateX(0.1em);
}

.cssbuttons-io-button:active .icon {
  transform: scale(0.95);
}

.card__content {
  height: 22rem;
}
</style>
