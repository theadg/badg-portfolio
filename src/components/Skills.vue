<template>
  <div class="pt-48 max-w-7xl m-center" id="skills">
    <div
      class="mt-10 text-center skills"
      data-aos="fade-up"
      data-aos-delay="100"
      data-aos-duration="800"
    >
      <h2 class="text-5xl dark:text-white">Skills</h2>
      <span class="text-sm f-gray dark:text-white">My Technical Level</span>
    </div>
    <div class="flex flex-col mt-20 skill-details lg:flex-row lg:gap-10">
      <div
        data-aos="fade-down"
        data-aos-duration="1000"
        data-aos-delay="200"
        class="bg-white lg:w-1/3 md:w-96 md:m-auto md:mb-16 card drop-shadow-2xl dark:bg-slate-800"
      >
        <h2 class="flex items-center pl-5 pt-7">
          <font-awesome-icon
            class="w-20 pr-3 fa-2xl f-blue"
            :icon="['fas', 'code']"
          />
          <div class="flex flex-col">
            <h2 class="text-xl dark:text-white">Frontend</h2>
            <span class="text-sm f-gray dark:text-white">Technologies</span>
          </div>
        </h2>
        <div
          class="grid grid-cols-4 gap-4 px-5 pt-10 m-auto description lg:px-10"
        >
          <div class="p-1 card-mini">
            <img
              src="https://www.logo.wine/a/logo/React_(web_framework)/React_(web_framework)-Logo.wine.svg"
              class="h-14"
              alt="ReactJs"
            />
            <span class="dark:text-white">ReactJs</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://mui.com/static/logo.png"
              class="h-14"
              alt="MaterialUI"
            />
            <span class="dark:text-white">MaterialUI</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://seeklogo.com/images/V/vuejs-logo-17D586B587-seeklogo.com.png"
              class="h-14"
              alt="VUEJS"
            />
            <span class="dark:text-white">VueJs</span>
          </div>

          <div class="p-1 card-mini">
            <img
              src="https://i2.wp.com/www.primefaces.org/wp-content/uploads/2019/12/primevue-logo.png?fit=300%2C300&ssl=1"
              class="h-14"
              alt="NuxtJs"
            />
            <span class="dark:text-white">PrimeVue</span>
          </div>

          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f1/Vitejs-logo.svg/410px-Vitejs-logo.svg.png"
              class="h-14"
              alt="NuxtJs"
            />
            <span class="dark:text-white">Vite</span>
          </div>

          <div class="p-1 card-mini">
            <img
              src="https://raw.githubusercontent.com/webpack/media/master/logo/icon-square-big.png"
              class="h-14"
              alt="NuxtJs"
            />
            <span class="dark:text-white">Webpack</span>
          </div>

          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/Tailwind_CSS_Logo.svg/600px-Tailwind_CSS_Logo.svg.png?20211001194333"
              class="h-14"
              alt="Tailwind"
            />
            <span class="dark:text-white">Tailwind</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://seeklogo.com/images/B/bootstrap-logo-3C30FB2A16-seeklogo.com.png"
              class="h-14"
              alt="Bootstrap"
            />
            <span class="dark:text-white">Bootstrap</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://cdn.worldvectorlogo.com/logos/styled-components-1.svg"
              class="h-14"
              alt="Bootstrap"
            />
            <span class="dark:text-white">Styled</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/130px-HTML5_logo_and_wordmark.svg.png"
              alt="HTML5"
              class="h-14"
            />
            <span class="dark:text-white">HTML5</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Typescript_logo_2020.svg/2048px-Typescript_logo_2020.svg.png"
              class="h-14"
              alt="CSS"
            />
            <span class="dark:text-white">TypeScript</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/JavaScript-logo.png/600px-JavaScript-logo.png?20120221235433"
              class="h-14"
              alt="JavaScript"
            />
            <span class="dark:text-white">JavaScript</span>
          </div>
        </div>
      </div>
      <div
        data-aos="fade-down"
        data-aos-duration="1000"
        data-aos-delay="400"
        class="bg-white lg:w-1/3 md:w-96 md:m-auto md:mb-16 card drop-shadow-2xl dark:bg-slate-800"
      >
        <h2 class="flex items-center pl-5 pt-7">
          <font-awesome-icon
            class="w-20 pr-3 fa-2xl f-blue"
            :icon="['fas', 'code-branch']"
          />
          <div class="flex flex-col">
            <h2 class="text-xl dark:text-white">Backend</h2>
            <span class="text-sm f-gray dark:text-white">Techonolgoies</span>
          </div>
        </h2>
        <div
          class="grid grid-cols-4 gap-4 px-5 pt-10 m-auto description lg:px-10"
        >
          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Laravel.svg/121px-Laravel.svg.png"
              class="h-14"
              alt="Laravel"
            />
            <span class="dark:text-white">Laravel</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://seeklogo.com/images/M/mongodb-logo-D13D67C930-seeklogo.com.png"
              alt="AWS"
            />
            <span class="dark:text-white">MongoDB</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://ajeetchaulagain.com/static/7cb4af597964b0911fe71cb2f8148d64/87351/express-js.png"
              class="h-14"
              alt="Docker"
            />
            <span class="dark:text-white">Express</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Node.js_logo.svg/590px-Node.js_logo.svg.png"
              class="h-14"
              alt="Laravel Lumen"
            />
            <span class="dark:text-white">Node</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://cdn-icons-png.flaticon.com/512/5968/5968332.png"
              class="h-14"
              alt="PHP"
            />
            <span class="dark:text-white">PHP</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://www.freepnglogos.com/uploads/logo-mysql-png/logo-mysql-mysql-logo-png-images-are-download-crazypng-21.png"
              class="h-14"
              alt="Mysql"
            />
            <span class="dark:text-white">MySQL</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/29/Postgresql_elephant.svg/640px-Postgresql_elephant.svg.png"
              class="h-14"
              alt="Mysql"
            />
            <span class="dark:text-white">PostgreSQL</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://cdn.worldvectorlogo.com/logos/prisma-4.svg"
              class="h-14"
              alt="CodeIgniter"
            />
            <span class="dark:text-white">Prisma</span>
          </div>

          <div class="p-1 card-mini">
            <img
              src="https://logowik.com/content/uploads/images/supabase-icon1721342077.logowik.com.webp"
              class="h-14"
              alt="CodeIgniter"
            />
            <span class="dark:text-white">Supabase</span>
          </div>

          <div class="p-1 card-mini">
            <img
              src="https://cdn.worldvectorlogo.com/logos/postman.svg"
              class="h-14"
              alt="CodeIgniter"
            />
            <span class="dark:text-white">Postman</span>
          </div>
        </div>
      </div>
      <div
        data-aos="fade-down"
        data-aos-duration="1000"
        data-aos-delay="600"
        class="bg-white lg:w-1/3 md:w-96 md:m-auto md:mb-16 card drop-shadow-2xl dark:bg-slate-800"
      >
        <h2 class="flex items-center pl-5 pt-7">
          <font-awesome-icon
            class="w-20 pr-3 fa-2xl f-blue"
            :icon="['fas', 'brain']"
          />
          <div class="flex flex-col">
            <h2 class="text-xl dark:text-white">Others</h2>
            <span class="text-sm f-gray dark:text-white">Acquired Skills</span>
          </div>
        </h2>
        <div
          class="grid grid-cols-4 gap-4 px-5 pt-10 m-auto description lg:px-10"
        >
          <div class="p-1 card-mini">
            <img
              src="https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png"
              class="h-14"
              alt="Git"
            />
            <span class="dark:text-white">Git</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://seeklogo.com/images/G/github-logo-5F384D0265-seeklogo.com.png"
              class="h-14"
              alt="GitHub"
            />
            <span class="dark:text-white">GitHub</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://cdn4.iconfinder.com/data/icons/logos-and-brands/512/44_Bitbucket_logo_logos-512.png"
              class="h-14"
              alt="GitHub"
            />
            <span class="dark:text-white">BitBucket</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://cdn.icon-icons.com/icons2/2699/PNG/512/atlassian_jira_logo_icon_170511.png"
              class="h-14"
              alt="Jira"
            />
            <span class="dark:text-white">Jira</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://cdn.sanity.io/images/599r6htc/localized/46a76c802176eb17b04e12108de7e7e0f3736dc6-1024x1024.png?w=670&h=670&q=75&fit=max&auto=format"
              class="h-14"
              alt="Figma"
            />
            <span class="dark:text-white">Figma</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c2/Adobe_XD_CC_icon.svg/2101px-Adobe_XD_CC_icon.svg.png"
              class="h-14"
              alt="Figma"
            />
            <span class="dark:text-white">XD</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
