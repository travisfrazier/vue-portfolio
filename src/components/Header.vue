<template>
    <header class="header section">
        <figure class="mobile-menu">
          <img
            onClick={this.toggleMenu}
            class="button"
            src='../assets/images/menu.png'
          />
        </figure>
        <nav>
          <ul>
            <li>
              <a href="#home">Home</a>
            </li>
            <li>
              <a href="#about">About</a>
            </li>
            <li>
              <a href="#projects">Projects</a>
            </li>
            <li>
              <a href="#contact">Contact</a>
            </li>
            <li>
              <a href="https://represent.io/travisfrazier" target="_blank">
                Resumé
              </a>
            </li>
          </ul>
        </nav>
        <div class="layer" />
        <p>
          Hello, My name is <strong class="name">Travis Frazier</strong> and I'm a
        </p>
        <h1>
          <strong>FRONT-END WEB DEVELOPER</strong>
        </h1>
        <p>creating modern and responsive web experiences.</p>
        <div class="social-links">
          <a href="https://www.instagram.com/travfrazier/">
            <i class="fa fa-instagram" />
          </a>
          <a href="https://www.facebook.com/travisfrazier7">
            <i class="fa fa-facebook" />
          </a>
          <a href="https://github.com/travisfrazier">
            <i class="fa fa-github" />
          </a>
          <a href="https://www.linkedin.com/in/travisf7/">
            <i class="fa fa-linkedin" />
          </a>
        </div>
        <a class="arrow-container">
          <i class="fa fa-angle-double-down arrow" />
        </a>
      </header>
</template>



<script>
export default {
  name: "Header",
  props: {
  },
  methods: {
  }
};
</script>

<style lang="scss" scoped>
h1 {
  overflow: hidden; /* Ensures the content is not revealed until the animation */
  border-right: .15em solid orange; /* The typwriter cursor */
  white-space: nowrap; /* Keeps the content on a single line */
  margin: 0 auto; /* Gives that scrolling effect as the typing happens */
  //letter-spacing: .15em; /* Adjust as needed */
  animation: 
    typing 3.5s steps(40, end),
    blink-caret .75s step-end infinite;
}

/* The typing effect */
@keyframes typing {
  from { width: 0 }
  to { width: 100% }
}

/* The typewriter cursor effect */
@keyframes blink-caret {
  from, to { border-color: transparent }
  50% { border-color: orange; }
}
header {
  background-image: url('../assets/images/laptop.jpg');
  background-size: cover;
  background-position: center;
  height: 100vh;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  nav {
    position: absolute;
    top: 0rem;
    width: 100%;
    display: flex;
    justify-content: flex-end;
    z-index: 999;
    @media only screen and (max-width: 768px) {
      display: none;
      justify-content: center;
      background-color: transparent;
      padding-top: 1.25rem;
      background-color: #212121;
    }
    ul {
      list-style-type: none;
      width: 25rem;
      padding-right: 3rem;
      z-index: 3;
      display: flex;
      justify-content: space-between;
      @media only screen and (max-width: 768px) {
        flex-direction: column;
        //justify-content: flex-start;
        align-items: flex-start;
        margin-top: 2.5rem;
      }
      li {
        @media only screen and (max-width: 768px) {
          padding: 0.5rem;
          font-size: 1.15rem;
          width: 100%;
        }
        a {
          color: #f5f5f5;
          @media only screen and (max-width: 768px) {
            padding-right: 90%;
          }
          &:visited {
            color: #f5f5f5;
          }
          &:hover {
            color: #ff3f80;
            //border-bottom: 1px solid #118aaf;
          }
        }
      }
    }
  }
  //Mobile Nav
  .mobile-menu {
    position: absolute;
    top: 1rem;
    z-index: 1000;
    display: none;
    margin: auto;
    @media only screen and (max-width: 768px) {
      display: block;
    }
    img {
      width: 2rem;
      height: 2rem;
    }
  }

  //Toggle menu
  .block {
    display: flex !important;
  }
  //end
  .layer {
    background-color: #000000ab;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
  h1 {
    z-index: 1;
    font-weight: 400;
    width: 100%;
    text-align: center;
    color: #f5f5f5;
    font-size: 5vw;
    margin: 0.25rem 0rem;
    padding-top: 0rem;
    @media only screen and (max-width: 812px) {
      //font-size: 2.4rem;
      font-size: 6vw;
      width: 95%;
    }
  }
  p {
    z-index: 1;
    font-size: 1.75vw;
    color: #f5f5f5;
    @media only screen and (max-width: 812px) and (min-width: 415px) {
      margin: 0.25rem;
    }
    @media only screen and (max-width: 600px) {
      font-size: 1.25rem;
      text-align: center;
      width: 95%;
    }
  }
  .social-links {
    z-index: 1;
    display: flex;
    width: 100%;
    justify-content: center;
    @media only screen and (max-width: 812px) and (min-width: 376px) {
      margin-top: 0.25rem;
    }
    a {
      display: inline-table;
      text-align: center;
      height: 35px;
      width: 35px;
      color: #fff;
      border-radius: 50%;
      border: 1px solid #3e50b4;
      margin: 0 0.5rem;
    }
    i {
      display: table-cell;
      vertical-align: middle;
      color: #3e50b4;
      text-shadow: 2px 2px 10px black;
    }
  }
  .arrow-container {
    display: flex;
    justify-content: center;
  }
  .arrow {
    color: #ffffffcb;
    //width: 3rem;
    z-index: 3;
    position: absolute;
    bottom: 2rem;
    font-size: 2rem;
    @media only screen and (max-width: 767px) and (min-width: 415px) {
      bottom: 0.75rem;
    }
  }
}
</style>