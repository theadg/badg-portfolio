<template>
  <div class="pt-20 max-w-7xl m-center" id="projects">
    <div
      class="mt-10 text-center about-me md:mt-32"
      data-aos="fade-up"
      data-aos-delay="100"
      data-aos-duration="800"
    >
      <h2 class="text-5xl dark:text-white">Portfolio</h2>
      <span class="text-sm f-gray dark:text-white">Recent Projects</span>
    </div>
    <div
      class="flex justify-center gap-10 details"
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
            class="bg-white rounded custom-card dark:bg-slate-800 drop-shadow-2xl w-80 h-96"
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
            <div class="flex flex-col justify-between p-2 card__content">
              <div class="flex flex-col gap-2">
                <div class="project-img">
                  <img
                    :src="project.project_logo"
                    alt=""
                    :class="`${project.class} thumbnail m-auto max-h-24 object-cover`"
                  />
                </div>
                <div class="pt-2 text-2xl font-semibold title dark:text-white">
                  {{ project.name }}
                </div>
                <div class="text-sm text-gray-400 description">
                  {{ project.description }}
                </div>
              </div>
              <div class="flex justify-center visit-link">
                <a
                  class="cursor-pointer cssbuttons-io-button bg-cyan-500 w-44"
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

<script lang="ts">
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
          name: "Carepulse",
          project_link: "https://carepulse-lake.vercel.app/",
          project_logo:
            "https://carepulse-lake.vercel.app/assets/icons/logo-full.svg",
          description: "Patient and Schedule Booking and Management Platform",
        },
        {
          name: "AMA Chatbot",
          project_link: "https://ask-me-anything-chat-bot.vercel.app/",
          project_logo:
            "https://media.istockphoto.com/id/1413286466/vector/chat-bot-icon-robot-virtual-assistant-bot-vector-illustration.jpg?s=612x612&w=0&k=20&c=ZSG3eqGPDJgIgFUIuVxID64uVUF3eqM3LrrDWtaKses=",
          description: "Chatbot Powered by Google Gemini",
        },
        {
          name: "Threads Clone",
          project_link: "https://threads-hazel.vercel.app/",
          project_logo:
            "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRdI_fwObzik_aoEpMpi4zjj69_F2gM4k7tpw&s",
          description: "Clone of Meta's Threads",
        },
        {
          name: "Pili-Pinas",
          project_link: "https://pili-pinas.onrender.com/",
          project_logo:
            "https://drive.google.com/thumbnail?sz=w1920&id=16zcPBc_Ag6Nv-NTg39WNUSHF_tdBNW7I",
          description: "Capstone Project Streamlining the travel experience",
        },
        {
          name: "Wordle Clone",
          project_link: "https://theadg.github.io/wordle-clone/",
          project_logo:
            "https://static01.nyt.com/images/2022/03/02/crosswords/alpha-wordle-icon-new/alpha-wordle-icon-new-square320-v3.png?format=pjpg&quality=75&auto=webp&disable=upscale",
          description: "Clone of the pandemic hit game",
        },
        {
          name: "The Do List",
          project_link: "https://theadg.github.io/todo-list/",
          project_logo:
            "https://static-00.iconduck.com/assets.00/check-mark-button-emoji-2048x2048-lq7rf7h8.png",
          description: "Essential CRUD Project",
        },

        {
          name: "Tic Tac Toe",
          project_link: "https://theadg.github.io/tic-tac-toe/",
          project_logo:
            "https://em-content.zobj.net/source/skype/289/o-button-blood-type_1f17e-fe0f.png",
          description: "A classic on the browser",
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
