<template>
  <aside class="sidebar" :class="{ active: isOpen }">
    <div class="sidebar-info">
      <figure class="avatar-box">
        <img src="/images/avatar.jpg" alt="Photo" width="80">
      </figure>

      <div class="info-content">
        <h1 class="name" title="Needhi Deshmukh">
          Needhi Deshmukh
        </h1>

        <p class="title text-center xl:block flex items-center justify-center gap-1">
          <span>Web Developer</span>
        </p>
      </div>

      <button class="info_more-btn" @click="isOpen = !isOpen">
        <span>Show Contacts</span>

        <ion-icon name="chevron-down" />
      </button>
    </div>

    <div class="sidebar-info_more">
      <div class="separator" />

      <ul class="contacts-list">

        <li class="contact-item">
          <div class="icon-box">
            <ion-icon name="folder" />
          </div>

          <div class="contact-info">
            <p class="contact-title">
              Resume
            </p>

            <a href="https://drive.google.com/file/d/1bDn35hD10zr66fe_KRbfMDLS8fD5iHuz/view?usp=drive_link" class="contact-link" target="_blank">Resume</a>
          </div>
        </li>


        <li class="contact-item">
          <div class="icon-box">
            <ion-icon name="logo-github" />
          </div>

          <div class="contact-info">
            <p class="contact-title">
              GitHub
            </p>

            <a href="https://github.com/needhideshmukh" class="contact-link" target="_blank">needhideshmukh</a>
          </div>
        </li>

  

        <li class="contact-item">
          <div class="icon-box">
            <ion-icon name="logo-linkedin" />
          </div>

          <div class="contact-info">
            <p class="contact-title">
              Linkedin
            </p>

            <a href="https://www.linkedin.com/in/needhideshmukh/" class="contact-link" target="_blank">Needhi Deshmukh</a>
          </div>
        </li>

        <li class="contact-item">
          <div class="icon-box">
            <ion-icon name="mail" />
          </div>

          <div class="contact-info">
            <p class="contact-title">
              Email
            </p>
            <nuxt-link to="mailto:needhideshmukh05@gmail.com"  target="_blank">
                 <address>needhideshmukh05 <br> @gmail.com</address>         
            </nuxt-link>

          </div>
        </li>
      </ul>

      <div class="separator" />

      <ul class="social-list">
        <li class="social-item">
  
            <ion-icon class="social-link"  name="sunny"></ion-icon>
            <span> {{ datee() }}</span>
    
        </li>
      </ul>
    </div>
  </aside>
</template>

<script >
let isOpen = ref(false)


export default{
  methods: {
  datee(){
    const current = new Date();
    const date = `${current.getDate()}`
  }
}
}


function toggleMenu() {
  isOpen = !isOpen
}



</script>
