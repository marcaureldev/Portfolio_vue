<script >
import Twitter from './assets/icons/Vector.svg'
import Card  from "./components/Card.vue";
import Work from "./components/Work.vue";
import CardTestimonials from "./components/CardTestimonials.vue";
export default {
  name:'App',
  components: {
    Card,
    Work,
    CardTestimonials,
  },

  data() {
    return {
      Twitter: Twitter,
    };
}
}

document.addEventListener('DOMContentLoaded', ()=> {
  const btn = document.querySelector('.btn')
const nav_content = document.querySelector('.nav_content')

btn.addEventListener('click', function()
{
  if(nav_content.classList.contains('hidden'))
  {
    nav_content.classList.remove('hidden')
  } else
  {
    nav_content.classList.add('hidden')
  }
})
})
</script>

<template>
  <div id="app">
      <header class="max-w-[70em] mx-auto">
        <div class="md:flex md:justify-between md:items-center p-7 text-center space-y-2 md:space-y-0">
            <div class="flex justify-between px-5">
              <img src="./assets/icons/logo.svg" alt="Logo">
              <img src="./assets/images/button_mobile.svg" alt="" class="md:hidden btn">
            </div>
              <nav class="md:flex gap-5 md:items-center space-y-2 md:space-y-0 hidden nav_content">

                  <ul class="md:flex gap-8 md:items-center space-y-5 md:space-y-0">
                      <li>About</li>
                      <li>Work</li>
                      <li>Testimonials</li>
                      <li>Contact</li>
                  </ul>
                  <img src="./assets/icons/Icon Button.svg" alt="" class="mx-auto">
                  <button class="bg-[#111827] text-white p-2 rounded-xl">Download CV</button>

              </nav>
        </div>
      </header>

      <section class="max-w-[70em] mx-auto p-8">
          <div class="flex flex-col-reverse lg:flex-row lg:justify-between lg:items-center  gap-10">
            <div class="space-y-6 max-w-[40em] mx-auto lg:mx-0 ">
            <h1 class="text-4xl font-bold">Hi, I’m Marc-Aurel 👋</h1>
            <p class="text-[#4B5563] text-[15px]">
              I'm a full stack developer (React.js & Node.js) with a focus on creating (and occasionally designing) 
              exceptional digital experiences that are fast, accessible, visually appealing, and responsive. Even 
              though I have been creating web applications for over 7 years, I still love it as if it was something new.
            </p>
            <p class="flex gap-2 items-center justify-center lg:justify-start">
              <img src="./assets/icons/localisation.svg" alt="">
              Parakou, Bénin
            </p>
            <p class="flex gap-2 items-center justify-center lg:justify-start">
              <img src="./assets/icons/point.svg" alt="">
              Available for new projects
            </p>
            <div class="flex gap-3 justify-center lg:justify-start">
              <img src="./assets/icons/github.svg" alt="">
              <img src="./assets/icons/figma_icon.svg" alt="">
              <img :src='Twitter' alt="">
            </div>
        </div>
        <img src="./assets/images/Pic Container.svg" alt="" class="mx-auto">
          </div>
      </section>

      <section class="bg-[#F9FAFB] sm:p-10">
         <div class="max-w-[70em] mx-auto">
          <p class="text-[#4B5563] bg-[#E5E7EB] max-w-[6em] mx-auto text-center p-1 rounded-xl">About me</p>
          <div class="lg:flex gap-28 lg:items-center p-5">
            <img src="./assets/images/pic_container.svg" alt="">
            <div class="text-[#4B5563] space-y-4">
                <h1 class="text-2xl font-bold text-black">Curious about me? Here you have it:</h1>
                <p>
                  I'm a passionate, self-proclaimed designer who specializes in full stack development (React.js & Node.js). 
                  I am very enthusiastic about bringing the technical and visual aspects of digital products to life. User experience, 
                  pixel perfect design, and writing clear, readable, highly performant code matters to me.
                </p>
                <p>
                  I began my journey as a web developer in 2015, and since then, I've continued to grow and evolve as a developer, 
                  taking on new challenges and learning the latest technologies along the way. Now, in my early thirties, 
                  7 years after starting my web development journey, I'm building cutting-edge web applications using modern technologies 
                  such as Next.js, TypeScript, Nestjs, Tailwindcss, Supabase and much more.
                </p>
                <p>
                  I am very much a progressive thinker and enjoy working on products end to end, from ideation all the way to development.
                </p>
                <p>
                  When I'm not in full-on developer mode, you can find me hovering around on twitter or on indie hacker, witnessing the journey 
                  of early startups or enjoying some free time. You can follow me on Twitter where I share tech-related bites and build in public, or you can follow me on GitHub.
                </p>
                <p>
                  Finally, some quick bits about me.
                </p>
                <div class="flex justify-around items-center">
                    <ul class="list-disc">
                      <li>B.E. in Computer Engineering</li>
                      <li>Full time freelancer</li>
                    </ul>
                    <ul class="list-disc">
                      <li>Avid learner</li>
                      <li>Aspiring indie hacker</li>
                    </ul>
                </div>
                <p>
                  One last thing, I'm available for freelance work, so feel free to reach out and say hello! I promise I don't bite 😉
                </p>
            </div>
          </div>
         </div>
      </section>


      <section class="max-w-[70em] mx-auto p-8 space-y-8">
          <p class="text-[#4B5563] bg-[#E5E7EB] max-w-[6em] mx-auto text-center p-1 rounded-xl">Skills</p>
          <p class="text-center">The skills, tools and technologies I am really good at:</p>
          <div class="grid grid-cols-3 md:grid-cols-4 lg:grid-cols-8 gap-8 text-[#4B5563] py-5">
              <div class="text-center">
                <img src="./assets/images/javascript.svg" alt="" class="mx-auto">
                Javascript
              </div>
              <div class="text-center">
                <img src="./assets/images/typescript.svg" alt="" class="mx-auto">
                Typescript
              </div>
              <div class="text-center">
                <img src="./assets/images/icon-react.svg" alt="" class="mx-auto">
                React
              </div>
              <div class="text-center">
                <img src="./assets/images/next.svg" alt="" class="mx-auto">
                Next.js
              </div>
              <div class="text-center">
                <img src="./assets/images/node.svg" alt="" class="mx-auto">
                Node.js
              </div>
              <div class="text-center">
                <img src="./assets/images/express.svg" alt="" class="mx-auto">
                Express.js
              </div>
              <div class="text-center">
                <img src="./assets/images/nest.svg" alt="" class="mx-auto">
                Nest.js
              </div>
              <div class="text-center">
                <img src="./assets/images/socket.svg" alt="" class="mx-auto">
                Socket.io
              </div>
              <div class="text-center">
                <img src="./assets/images/postgreesql.svg" alt="" class="mx-auto">
                PostgreSQL
              </div>
              <div class="text-center">
                <img src="./assets/images/mongo.svg" alt="" class="mx-auto">
                MongoDB
              </div>
              <div class="text-center">
                <img src="./assets/images/saas.svg" alt="" class="mx-auto">
                Sass/Scss
              </div>
              <div class="text-center">
                <img src="./assets/images/tailwind.svg" alt="" class="mx-auto">
                Tailwindcss
              </div>
              <div class="text-center">
                <img src="./assets/images/figma.svg" alt="" class="mx-auto">
                Figma
              </div>
              <div class="text-center">
                <img src="./assets/images/cypress.svg" alt="" class="mx-auto">
                Cypress.js
              </div>
              <div class="text-center">
                <img src="./assets/images/storybook.svg" alt="" class="mx-auto">
                Storybook
              </div>
              <div class="text-center">
                <img src="./assets/images/git.svg" alt="" class="mx-auto">
                Git
              </div>
          </div>
      </section>


      <section class="bg-[#F9FAFB]">
        <div class="max-w-[70em] mx-auto p-10 space-y-8">
          <div class="space-y-5">
              <p class="text-[#4B5563] bg-[#E5E7EB] max-w-[6em] mx-auto text-center p-1 rounded-xl">Experience</p>
              <p class="text-center">Here is a quick summary of my most recent experiences:</p>
              <Card v-for="(item, index) in 3" :key="index"/>
          </div>
        </div>
      </section>

      
      <section class="max-w-[70em] mx-auto p-10 space-y-10">
          <div>
              <p class="text-[#4B5563] bg-[#E5E7EB] max-w-[6em] mx-auto text-center p-1 rounded-xl">Work</p>
              <p class="text-center">Some of the noteworthy projects I have built:</p>
              <Work v-for="(item, index) in 3" :key="index"/>
          </div>
      </section>

      <section class="bg-[#F9FAFB]">
        <div class="space-y-10 max-w-[70em] mx-auto p-10">
             <p class="text-[#4B5563] bg-[#E5E7EB] max-w-[6em] mx-auto text-center p-1 rounded-xl">Testimonials</p>
             <p class="text-center">Nice things people have said about me:</p>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
               <CardTestimonials v-for="(item, index) in 3" :key="index"/>
            </div>
        </div>
      </section>

      <section class="space-y-10 max-w-[70em] mx-auto p-20">
          <div class="space-y-5">
            <p class="text-[#4B5563] bg-[#E5E7EB] max-w-[8em] mx-auto text-center p-1 rounded-xl">Get in touch</p>
             <p class="text-center max-w-[30em] mx-auto text-[#4B5563]">What’s next? Feel free to reach out to me if you're looking for a developer, have a query, or simply want to connect.</p>
             <p class="flex gap-2 justify-center lg:text-xl font-bold"> <img src="./assets/icons/mail.svg" alt=""> reachsagarshah@gmail.com <img src="./assets/icons/paste_icon.svg" alt=""> </p>
             <p class="flex gap-2 justify-center lg:text-xl font-bold"> <img src="./assets/icons/phone_icon.svg" alt=""> +91 8980500565<img src="./assets/icons/paste_icon.svg" alt=""> </p>
             <p class="text-center text-[#4B5563]">You may also find me on these platforms!</p>
             <div class="flex gap-3 justify-center">
                <img src="./assets/icons/github.svg" alt="">
                <img src="./assets/icons/figma_icon.svg" alt="">
                <img :src='Twitter' alt="">
            </div>
          </div>
      </section>
      <footer class="bg-[#E5E7EB]">
        <p class="text-center text-[#4B5563] p-3">&copy;2023 | Designed and coded with ❤️️ by Sagar Shah</p>
      </footer>
    </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
#app {
  font-family: 'Inter', sans-serif; }

</style>