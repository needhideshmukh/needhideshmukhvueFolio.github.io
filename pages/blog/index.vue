<script setup>
useHead({
  title: 'Blog',
})
</script>

<template>
  <article class="blog active" data-page="blog">
    <header>
      <h2 class="h2 article-title">
        {{ $t('pageTitles.blog') }}
      </h2>
    </header>

    <section class="blog-posts">
      <ul class="blog-posts-list">
        <!-- <li class="blog-post-item">
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
        </li> -->

        <!-- <li class="blog-post-item">
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
</template>
