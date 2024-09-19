<template>
  <div class="pt-20 pb-20 max-w-7xl m-center" id="about">
    <div
      class="mt-10 text-center about-me md:mt-32"
      data-aos="fade-up"
      data-aos-delay="100"
      data-aos-duration="800"
    >
      <h2 class="text-5xl dark:text-white">About Me</h2>
      <span class="text-sm f-gray dark:text-white">Personal</span>
    </div>
    <div
      class="flex flex-col-reverse mt-20 details md:flex-col-reverse lg:flex-row"
    >
      <div
        class="mt-12 image lg:w-3/6 lg:m-auto"
        data-aos="fade-right"
        data-aos-delay="500"
        data-aos-duration="500"
      >
        <img
          class="w-11/12 m-auto rounded-md drop-shadow-lg lg:m-0 h-1/2"
          src="https://drive.google.com/thumbnail?sz=w1920&id=1uaPHrrD1Fm0pSAR9wpSzyTOHke-vjTdW"
          alt=""
        />
      </div>
      <div
        class="flex flex-col information lg:w-3/6"
        data-aos="fade-right"
        data-aos-delay="1200"
        data-aos-duration="500"
      >
        <div
          class="text-lg text-center cover-letter f-gray pb-7 dark:text-white lg:text-left md:justify-center lg:justify-start"
        >
          I have always been curious about a lot of things since I was a child.
          I ask the stupidest questions, even up until now. I tend to ask
          <span class="italic">"how can this be better"</span> and
          <span class="italic">"why does this work" </span>
          to almost everything. My curiosity brought me where I am now, to
          solving problems and making the world a better place through the use
          of technology.
        </div>
        <div
          class="flex justify-center gap-10 text-center summary-experience lg:justify-start md:gap-5"
        >
          <div class="w-2/12 years-exp">
            <h2 class="text-3xl font-extrabold f-dark-blue dark:text-blue-500">
              18+
            </h2>
            <span class="text-sm f-gray dark:text-white"
              >Months of Experience</span
            >
          </div>
          <div class="w-2/12 projects">
            <h2 class="text-3xl font-extrabold f-dark-blue dark:text-blue-500">
              6+
            </h2>
            <span class="text-sm f-gray dark:text-white"
              >Joined Competitions</span
            >
          </div>
          <div class="w-2/12 companies-worked">
            <h2 class="text-3xl font-extrabold f-dark-blue dark:text-blue-500">
              10+
            </h2>
            <span class="text-sm f-gray dark:text-white"
              >Projects Completed</span
            >
          </div>
        </div>
        <div class="pt-10 resume">
          <button class="flex items-center m-auto btn-accent lg:m-0">
            <a
              href="https://drive.google.com/file/d/1HDoHReJZCEs5D79Jt_S-oGWSd6vT_RWV/view"
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
