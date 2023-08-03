<script setup>
useHead({
  title: 'Resume',
})
</script>

<template>
  <article class="resume active" data-page="resume">
    <header>
      <h2 class="h2 article-title">
        {{ $t('pageTitles.resume') }}
      </h2>
    </header>

    <section class="timeline">
      <ol class="timeline-list">



        <li class="timeline-item">
          <h4 class="h4 timeline-item-title">
            Mintbagg
          </h4>
          <span>Jan 2023 — Jul 2023</span>
          <p class="timeline-item-desc">
            Remote
          </p>
          <p class="timeline-text">
            Software Developer Engineer
          </p>
        </li>
        
        <br>


        <li class="timeline-item">
          <h4 class="h4 timeline-item-title">
            LTIMindtree
          </h4>
          <span>Feb 2023 — Apr 2023</span>
          <p class="timeline-item-desc">
            Remote
          </p>
          <p class="timeline-text">
            Graduate Engineer Trainee (Java)
          </p>
        </li>
        <br> 


        <li class="timeline-item">
          <h4 class="h4 timeline-item-title">
            BdigitaU
          </h4>
          <span>May 2021 — Sep 2021</span>
          <p class="timeline-item-desc">
            Remote
          </p>
          <p class="timeline-text">
            Content Writer
          </p>
        </li>
        <br> 


        <li class="timeline-item">
          <h4 class="h4 timeline-item-title">
            Sachal Technology llp
          </h4>
          <span>Aug 2021 — Aug 2021</span>
          <p class="timeline-item-desc">
            Remote
          </p>
          <p class="timeline-text">
            Game Developer
          </p>
        </li>
        <br>



        <li class="timeline-item">
          <h4 class="h4 timeline-item-title">
            Aparasoft
          </h4>
          <span>  Mar 2021 — Apr 2021</span>
          <p class="timeline-item-desc">
            Remote
          </p>
          <p class="timeline-text">
            Frontend Developer
          </p>
        </li>



<!-- 
        <li class="timeline-item">
          <h4 class="h4 timeline-item-title">
            Company
          </h4>
          <span>From — Until</span>
          <p class="timeline-item-desc">
            Location
          </p>
          <p class="timeline-text">
            Position
          </p>
        </li> -->



      </ol>
    </section>

    <!-- <section class="skill">
      <ul class="skills-list content-card">
        <li class="skills-item">
          <div class="title-wrapper">
            <h5 class="h5">
              Your Skill
            </h5>
            <data value="90">90%</data>
          </div>

          <div class="skill-progress-bg">
            <div class="skill-progress-fill" style="width: 90%;" />
          </div>
        </li>

      </ul>
    </section> -->


        <section class="skill">
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
          </div>
        </li>

      </ul>
    </section>
    
  </article>
</template>
