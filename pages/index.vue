<template>
  <article class="about active" data-page="about">
    <header>
      <h2 class="h2 article-title">
        {{ $t('pageTitles.about') }}
      </h2>
    </header>

    <section class="about-text">
      <ul class="about-list">
        <AboutItem v-for="about in about" :key="about.id" :about="about" />
      </ul>
    </section>

    
    <!-- testimonials -->

   <!-- <section class="testimonials">
      <h3 class="h3 testimonials-title">
        Testimonials
      </h3>

      <ul class="testimonials-list has-scrollbar">
        <li v-for="testimonial in testimonials" :key="testimonial.id" class="testimonials-item" @click="showTestimonial(testimonial.id)">
          <div class="content-card">
            <figure class="testimonials-avatar-box">
              <img :src="testimonial.image" alt="Daniel lewis" width="60">
            </figure>

            <h4 class="h4 testimonials-item-title">
              {{ testimonial.title }}
            </h4>

            <div class="testimonials-text">
              <p>{{ locale === 'en' ? testimonial.content?.en : testimonial.content?.id_ID }}</p>
            </div>
          </div>
        </li>
      </ul>
    </section> -->

    <!-- testimonials modal -->

    <!-- <div class="modal-container" :class="{ active: activeModal }">
      <div v-show="activeModal" class="overlay" :class="{ active: activeOverlay }" />

      <section class="testimonials-modal">
        <button class="modal-close-btn" @click="closeTestimonaial">
          <ion-icon name="close-outline" />
        </button>

        <div class="flex gap-5 mb-5 justify-start items-center">
          <div class="modal-avatar-box">
            <img :src="testimonialItem.image" alt="Daniel lewis" width="80">
          </div>

          <div class="modal-content">
            <h4 class="h3 modal-title">
              {{ testimonialItem.title }}
            </h4>
            <time datetime="2021-06-14">14 June, 2021</time>
          </div>
        </div>

        <div class="flex gap-5 items-start">
          <img class="my-auto hidden md:block" src="/images/icon-quote.svg" alt="quote icon">
          <p class="text-justify text-gray-400 text-sm md:text-md" v-html="locale === 'en' ? testimonialItem.content?.en : testimonialItem.content?.id_ID" />
        </div>
        <div class="mt-2 flex justify-end text-sm text-gray-600 italic">
          Company Co.
        </div>
      </section>
    </div> -->

    <!-- clients -->

    <section class="clients">
      <h5 class="h5 clients-title">
        Hey there! <br>I am Needhi Deshmukh, a frontend developer with a spectacular Vue. I try finding Nuxt great opportunites to solve new problems and shape my skills. 
        <br><br>
         In the dynamic world of web development, I harness the power of Vue.js, Nuxt.js, and Node.js to craft captivating user interfaces and seamless web experiences. Complemented by Express.js and SpringBoot, I build robust server-side applications and RESTful APIs for cohesive data communication.
         <br><br>
         With a focus on efficiency and collaboration, I utilize Git, GitHub, and Maven for streamlined version control and project management. Postman ensures thorough API testing, while MySQL Workbench empowers seamless database interactions.

To enhance user experiences, I rely on jQuery and Bootstrap to create interactive and responsive web applications. Understanding the significance of service technologies, I delve into ServiceNow and Salesforce to revolutionize business workflows and customer experiences.
<br><br>
With a solid foundation in Java, I have been practicing Data Structures and Algorithms (DSA), enabling me to develop robust solutions to complex problems. Embracing the versatility of Python and C/C++, I leverage these languages for diverse applications, from rapid prototyping to performance-critical tasks.
<br><br>
So, there you have it! That's the story of how I fell in love with coding and became a software developer. But before you go, here's a lighthearted joke to brighten your day:
<br><br>
Why do programmers always mix up Christmas and Halloween?
<br><br>
Because Oct 31 equals Dec 25 in hexadecimal! 🎃🎄
</h5>

      <!-- <ul class="clients-list has-scrollbar">
        
        <li class="clients-item service-item">
          <img class="service-icon-box" src="../public/images/loading.png" alt="" srcset="">
          
        </li>


        <li class="clients-item service-item">
          
        </li>
      </ul> -->
    </section>
  </article>
</template>

<script setup>
// import { useI18n } from 'vue-i18n'
// import { Icon } from '@iconify/vue';

// useHead({
// })

// onMounted(() => {
//   useLocaleStore()
// })

// const { locale } = useI18n({ useScope: 'global' })

// /* Testimonials */
// const { data: testimonials } = await useFetch('/api/testimonials')

// const testimonialItem = ref({})
// const activeModal = ref(false)
// const activeOverlay = ref(false)

// function showTestimonial(id) {
//   testimonialItem.value = testimonials.value.find(item => item.id === id)
//   activeModal.value = true
//   activeOverlay.value = true
// }

// function closeTestimonaial() {
//   testimonialItem.value = {}
//   activeModal.value = false
//   activeOverlay.value = false
// }
// /* Testimonials */

// /* Services */
// const { data: services } = await useFetch('/api/services')

// /* Services */
// const { data: about } = await useFetch('/api/about')
</script>
