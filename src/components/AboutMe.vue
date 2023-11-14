<template>
  <div class="max-w-7xl m-center pt-20 pb-20" id="about">
    <div
      class="about-me text-center mt-10 md:mt-32"
      data-aos="fade-up"
      data-aos-delay="100"
      data-aos-duration="800"
    >
      <h2 class="text-5xl dark:text-white">About Me</h2>
      <span class="f-gray text-sm dark:text-white">Personal</span>
    </div>
    <div
      class="details flex mt-20 md:flex-col-reverse lg:flex-row flex-col-reverse"
    >
      <div
        class="image lg:w-3/6 mt-12 lg:m-auto"
        data-aos="fade-right"
        data-aos-delay="500"
        data-aos-duration="500"
      >
        <img
          class="w-11/12 rounded-md drop-shadow-lg m-auto lg:m-0 h-1/2"
          src="https://drive.google.com/uc?id=1uaPHrrD1Fm0pSAR9wpSzyTOHke-vjTdW"
          alt=""
        />
      </div>
      <div
        class="information lg:w-3/6 flex flex-col"
        data-aos="fade-right"
        data-aos-delay="1200"
        data-aos-duration="500"
      >
        <div
          class="cover-letter f-gray text-lg pb-7 dark:text-white text-center lg:text-left md:justify-center lg:justify-start"
        >
          I have always been curious about a lot of things since I was a child.
          I ask the stupidest questions, even up until now. I tend to ask 
          <span class="italic">"how can this be better"</span> and 
          <span class="italic">"why does this work" </span>  
          to almost everything. My curiosity brought me where I am now, to solving 
          problems and making the world a better place through the use of technology.
        </div>
        <div
          class="summary-experience flex text-center justify-center lg:justify-start gap-10 md:gap-5"
        >
          <div class="years-exp w-2/12">
            <h2 class="text-3xl f-dark-blue font-extrabold dark:text-blue-500">
              12+
            </h2>
            <span class="text-sm f-gray dark:text-white"
              >Months of Experience</span
            >
          </div>
          <div class="projects w-2/12">
            <h2 class="text-3xl f-dark-blue font-extrabold dark:text-blue-500">
              6+
            </h2>
            <span class="text-sm f-gray dark:text-white"
              >Joined Competitions</span
            >
          </div>
          <div class="companies-worked w-2/12">
            <h2 class="text-3xl f-dark-blue font-extrabold dark:text-blue-500">
              4+
            </h2>
            <span class="text-sm f-gray dark:text-white">Projects Ciompleted</span>
          </div>
        </div>
        <div class="resume pt-10">
          <button class="btn-accent flex items-center m-auto lg:m-0">
            <a
              href="https://drive.google.com/file/d/15cKyzNhxmUlj0N73axnwN3Sthp9hN9mx/view"
              target="_blank"
            >
              Download CV&nbsp;
              <span
                ><font-awesome-icon
                  class="w-4"
                  :icon="['fas', 'arrow-circle-down']"
              /></span>
            </a>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>
