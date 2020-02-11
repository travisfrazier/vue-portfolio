<template>
    <section id="projects" class="projects section">
    <div class="section-heading">
      <h2>My Latest Projects</h2>
    </div>
    <p class="project-disclaimer">
      *Projects below were built by me without the use of jQuery. Hover each for
      a description. They are fully responsive with media queries.
    </p>
    <div class="projects_container">
      <div 
        data-aos="fade-right" 
        class="project project-two"
      >
        <a href="https://emanatesummit.com" target="_blank">
          <img src='../assets/images/projects/emanate.png'/>
          <div class="project-inner">
            <div class="project-info">
              <h3>Emanate Summit</h3>
              <p>
                Designed and Developed freelance client website (work in
                progress). Built with: ReactJS and SASS.
              </p>
              <span>View Site</span>
            </div>
          </div>
        </a>
      </div>
      <div 
        data-aos="fade-up" 
        class="project project-two"
      >
        <a
          href="https://travisfrazier.github.io/flashcards-vue/"
          target="_blank"
        >
          <img src='../assets/images/projects/flash.png' />
          <div class="project-inner">
            <div class="project-info">
              <h3>Vue.js Flash Card App</h3>
              <p>
                Developed single page flash card app. Built with: Vue.js, HTML5,
                and SASS.
              </p>
              <span>View Site</span>
            </div>
          </div>
        </a>
      </div>
      <div 
        data-aos="fade-left" 
        class="project project-two"
      >
        <a href="https://codepen.io/travisfrazier/full/bKyzep/" target="_blank">
          <img src='../assets/images/projects/weather.png' />
          <div class="project-inner">
            <div class="project-info">
              <h3>Vanilla JS Weather App</h3>
              <p>
                Designed and Developed a single page weather app. Built with:
                Vanilla JavaScript, Fetch API, and SASS.
              </p>
              <span>View Site</span>
            </div>
          </div>
        </a>
      </div>
      <div 
        data-aos="fade-right" 
        class="project project-two"
      >
        <a href="https://reactlistapp.netlify.com" target="_blank">
          <img src='../assets/images/projects/list.png' />
          <div class="project-inner">
            <div class="project-info">
              <h3>React.js List App</h3>
              <p>
                Designed and Developed a single page to-do app. Built with:
                React.js and SASS.
              </p>
              <span>View Site</span>
            </div>
          </div>
        </a>
      </div>
      <div 
        data-aos="fade-down" 
        class="project project-two"
      >
        <a href="https://themimosasnailbar.com" target="_blank">
          <img src='../assets/images/projects/mimosas-new.png' />
          <div class="project-inner">
            <div class="project-info">
              <h3>Mimosas Nail Bar (work in progress)</h3>
              <p>
                Developed client website following design spec. Incorporates a
                Headless CMS for content updates. Built with: SASS, HTML5,
                Vanilla JavaScript, VueJS, and Jekyll.
              </p>
              <span>View Site</span>
            </div>
          </div>
        </a>
      </div>
      <div 
        data-aos="fade-left" 
        class="project project-two"
      >
        <a href="https://movie-sales.netlify.com/" target="_blank">
          <img src='../assets/images/projects/sales.png' />
          <div class="project-inner">
            <div class="project-info">
              <h3>React Graph</h3>
              <p>
                Designed and Developed movie sales mock app. Built
                with: ReactJS and SASS. Incorporates the Recharts composable charting library.
              </p>
              <span>View Site</span>
            </div>
          </div>
        </a>
      </div>
      <div 
        data-aos="fade-right" 
        class="project project-two"
      >
        <a href="https://queensboro.com" target="_blank">
          <img src='../assets/images/projects/queensboro.png' />
          <div class="project-inner">
            <div class="project-info">
              <h3>Queensboro Shirt Company</h3>
              <p>
                Designed and Developed aspects for Queensboro.com. Built with:
                HTML5, CSS3, JavaScript, jQuery, and Bootstrap.
              </p>
              <span>View Site</span>
            </div>
          </div>
        </a>
      </div>
      <div 
        data-aos="fade-up" 
        class="project project-two"
      >
        <a href="https://travisfrazier.github.io/vue-drum-pad/" target="_blank">
          <img src='../assets/images/projects/mpc-kit.png' />
          <div class="project-inner">
            <div class="project-info">
              <h3>Vue.js Drum Pad</h3>
              <p>
                Designed and Developed a single page drum pad application. Built
                with: Vue.js CDN, SASS, and HTML5.
              </p>
              <span>View Site</span>
            </div>
          </div>
        </a>
      </div>
      <div 
        data-aos="fade-left" 
        class="project project-two"
      >
        <a href="https://travisfrazier.github.io/matchgame/" target="_blank">
          <img src='../assets/images/projects/guess.png' />
          <div class="project-inner">
            <div class="project-info">
              <h3>Vanilla JS Match Game</h3>
              <p>
                Developed this match game application. Built with: Vanilla
                JavaScript, Bootstrap 4, and custom CSS.
              </p>
              <span>View Site</span>
            </div>
          </div>
        </a>
      </div>
    </div>
  </section>
</template>

<script>
    export default {
      name: 'Project'
        
    }
</script>

<style lang="scss" scoped>
.projects {
  background-color: #212121;
  padding-bottom: 3rem;
  overflow: scroll;
}

a {
  color: black;
  overflow: hidden;
  &:visited {
    color: black;
  }
}

.project-inner {
  position: absolute;
  display: flex;
  justify-content: center;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100.1%;
  opacity: 0;
  transition: 0.5s ease;
  background-color: #3e50b4e1;
}

.project {
  width: 100%;
  position: relative;
  overflow: hidden;
  img {
    width: 100%;
    opacity: 1;
    transition: 0.5s ease;
    backface-visibility: hidden;
  }
  .project-info {
    position: absolute;
    text-align: center;
    top: 25%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    h3 {
      margin: 0 auto;
      color: white;
    }
    p {
      color: #ffffffce;
      width: 90%;
      margin-right: auto;
      margin-left: auto;
      font-weight: 500;
      line-height: 1.5;
    }
    span {
      color: #ffffff;
    }
  }
}

.project-disclaimer {
  width: 90%;
  margin-top: -1rem;
  text-align: center;
  margin-right: auto;
  margin-left: auto;
  color: #ffffff8e;
}

.project:hover img {
  opacity: 0.3s;
  transform: scale(1.04);
}

.project:hover .project-inner {
  opacity: 1;
}

.projects_container {
  overflow: scroll;
  display: grid;
  padding-left: 1rem;
  padding-right: 1rem;
  padding-bottom: 3rem;
  grid-template-columns: repeat(auto-fit, minmax(25%, 1fr));
  @media only screen and (max-width: 1100px) {
    grid-template-columns: repeat(auto-fit, minmax(325px, 1fr));
  }
  grid-gap: 1rem;
}
</style>