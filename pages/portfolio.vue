<template>
  <article class="portfolio active" data-page="portfolio">
    <header>
      <h2 class="h2 article-title">
        {{ $t('pageTitles.portfolio') }}
      </h2>
    </header>

    <article class="blog active" data-page="blog">


    <section class="blog-posts">
      <ul class="blog-posts-list">
        <li class="blog-post-item">
          <a href="https://bit.ly/ADLink-Docs">

            <figure class="blog-banner-box">
              <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1685698726479/4120633e-1475-4696-af64-31a9296696dd.png?w=1600&h=840&fit=crop&crop=entropy&auto=compress,format&format=webp" alt="ADLink Documentation" loading="lazy">
            </figure>

            <div class="blog-content">

              <div class="blog-meta">
                <p class="blog-category">Docs</p>

                <span class="dot" />

                <time datetime="2023-06-2">June 2, 2023</time>
              </div>

              <h3 class="h3 blog-item-title">ADLink Documentation</h3>

              <p class="blog-text">
                A perfect custom alternative for linktree, bio and other shortner platform.
              </p>

            </div>

          </a>
        </li>

        <li class="blog-post-item">
          <a href="https://blog.agcrisbp.my.id/posts/cara-install-phpmyadmin-di-android-menggunakan-termux">

            <figure class="blog-banner-box">
              <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1685699212595/40c994c9-0d1a-4eba-a82b-76c5da81683f.png?w=1600&h=840&fit=crop&crop=entropy&auto=compress,format&format=webp" alt="Cara Install PHPMyAdmin Di Android Menggunakan Termux" loading="lazy">
            </figure>

            <div class="blog-content">

              <div class="blog-meta">
                <p class="blog-category">Guide</p>

                <span class="dot" />

                <time datetime="2023-05-21">May 21, 2023</time>
              </div>

              <h3 class="h3 blog-item-title">Cara Install PHPMyAdmin Di Android Menggunakan Termux</h3>

              <p class="blog-text">
                PHPMyAdmin adalah alat yang digunakan untuk mengelola database yang dapat diakses melalui web.
              </p>
            </div>
          </a>
        </li>



<!-- 
        <li class="blog-post-item">
          <a href="https://blog.agcrisbp.my.id/posts/cara-install-phpmyadmin-di-android-menggunakan-termux">

            <figure class="blog-banner-box">
              <img src="https://cdn.hashnode.com/res/hashnode/image/upload/v1685699212595/40c994c9-0d1a-4eba-a82b-76c5da81683f.png?w=1600&h=840&fit=crop&crop=entropy&auto=compress,format&format=webp" alt="Cara Install PHPMyAdmin Di Android Menggunakan Termux" loading="lazy">
            </figure>

            <div class="blog-content">

              <div class="blog-meta">
                <p class="blog-category">Guide</p>

                <span class="dot" />

                <time datetime="2023-05-21">May 21, 2023</time>
              </div>

              <h3 class="h3 blog-item-title">Cara Install PHPMyAdmin Di Android Menggunakan Termux</h3>

              <p class="blog-text">
                PHPMyAdmin adalah alat yang digunakan untuk mengelola database yang dapat diakses melalui web.
              </p>
            </div>
          </a>
        </li> -->
      </ul>
    </section>
  </article>


  <!-- -------------------------------- -->

    

    <!-- <section class="projects">
      <ul class="filter-list">
        <li class="filter-item">
          <button :class="{ active: activeCategory === 0 }" @click="changeFilter(0)">
            All
          </button>
        </li>

        <li v-for="category in categories" :key="category.id" class="filter-item" @click="changeFilter(category.id)">
          <button :class="{ active: activeCategory === category.id }">
            {{ locale === 'en' ? category.title?.en : category.title?.id_ID }}
          </button>
        </li>
      </ul>

      <div class="filter-select-box">
        <button :class="{ active: filterMenu }" class="filter-select" @click="filterMenu = !filterMenu">
          <div class="select-value">
            {{ activeCategory !== 0 ? (locale === 'en' ? activeCategoryName?.en : activeCategoryName?.id_ID) : 'Select Category' }}
          </div>

          <div class="select-icon">
            <ion-icon name="chevron-down" />
          </div>
        </button>

        <ul class="select-list">
          <li class="select-item">
            <button @click="changeFilter(0)">
              All
            </button>
          </li>

          <li v-for="category in categories" :key="category.id" class="select-item">
            <button @click="changeFilter(category.id)">
              {{ locale === 'en' ? category.title?.en : category.title?.id_ID }}
            </button>
          </li>
        </ul>
      </div>

      <ul class="project-list">
        <li v-for="project in projectList" :key="project.id" :class="{ active: activeCategory === project.category.id || activeCategory === 0 }" class="project-item">
          <a class="cursor-pointer" @click="showItem(project.id)">

            <figure class="project-img">
              <div class="project-item-icon-box">
                <ion-icon name="eye-outline" />
              </div>

              <img :src="project.image" :alt="project.title" loading="lazy">
            </figure>

            <h3 class="project-title">{{ project.title }}</h3>

            <p class="project-category">{{ locale === 'en' ? project.category.title?.en : project.category.title?.id_ID }}</p>

          </a>
        </li>
      </ul>

      <div class="modal-container" :class="{ active: activeModal }">
        <div v-show="activeModal" class="overlay" :class="{ active: activeOverlay }" />

        <section class="testimonials-modal block">
          <button class="modal-close-btn" @click="closeItem">
            <ion-icon name="close-outline" />
          </button>

          <div>
            <figure>
              <img :src="activeItem.image" class="rounded-lg" :alt="activeItem.title">
            </figure>
          </div>

          <div class="modal-content space-y-3 mt-4">
            <h4 class="h3 modal-title">
              {{ activeItem.title }}
            </h4>

            <small class="flex items-center justify-start gap-2 text-gray-500">
              <Icon icon="foundation:calendar" /><span>{{ locale === 'en' ? activeItem.category?.date?.en : activeItem.category?.date?.id_ID }}</span> | <Icon icon="dashicons:category" /><span>{{ locale === 'en' ? activeItem.category?.title?.en : activeItem.category?.title?.id_ID }}</span> | <Icon icon="ri:search-eye-line" /><a :href="activeItem.url" target="_blank">{{ locale === 'en' ? activeItem.desc?.en : activeItem.desc?.id_ID }}</a>
            </small>

            <p class="text-justify" v-html="locale === 'en' ? activeItem.content?.en : activeItem.content?.id_ID" />
          </div>
        </section>
      </div>
    </section> -->
    
    <!-- <section class="skill">
      <ul class="skills-list content-card">
        <li class="skills-item">
          <div class="title-wrapper">
            <h1 class="h5">
              Here is my Resume 
              <br> <br>
              <div class="contact-info">
                <a href="https://drive.google.com/file/d/1bDn35hD10zr66fe_KRbfMDLS8fD5iHuz/view?usp=drive_link" class="contact-link" target="_blank"><h2 class="h2 resume-color">View Resume <Icon class="iconColour" icon="fa fa-file-code-o" /></h2></a>
              </div>
           </h1>
           
            <data value="90">90%</data>
          </div>

          <div class="skill-progress-bg">
            <div class="skill-progress-fill" style="width: 90%;" />
          </div>
        </li>

      </ul>
    </section> -->
  </article>
</template>

<script setup>
//  import { useI18n } from 'vue-i18n'
// import Flicking from '@egjs/vue3-flicking'
import '@egjs/vue3-flicking/dist/flicking.css'
import { Icon } from '@iconify/vue';

// useHead({
//   title: 'Portfolio',
// })

// const { locale } = useI18n({ useScope: 'global' })
// const { data: projects } = await useFetch('/api/projects')
// const { data: categories } = await useFetch('/api/categories')

// const projectList = [...projects.value]
// const activeCategory = ref(0)
// const filterMenu = ref(false)
// const activeCategoryName = ref('')

// function changeFilter(id) {
//   activeCategory.value = id
//   if (id !== 0)
//     activeCategoryName.value = categories.value.find(item => item.id === id).title

//   filterMenu.value = !filterMenu.value
// }

// const activeItem = ref({})
// const activeModal = ref(false)
// const activeOverlay = ref(false)

// function showItem(id) {
//   activeItem.value = projects.value.find(item => item.id === id)
//   activeModal.value = true
//   activeOverlay.value = true
// }

// function closeItem() {
//   activeItem.value = {}
//   activeModal.value = false
//   activeOverlay.value = false
// }
</script>


