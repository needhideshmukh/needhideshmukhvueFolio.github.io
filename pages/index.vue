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

</script>
