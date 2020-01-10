<template>
  <footer class="footer">
    <div class="container">
      <div class="social-links">
        <a href="https://www.instagram.com/travfrazier/">
          <i class="fa fa-instagram" />
        </a>
        <a href="https://www.facebook.com/travisfrazier7">
           <i><font-awesome :icon="['fab', 'facebook']"/></i>
        </a>
        <a href="https://github.com/travisfrazier">
          <i><font-awesome :icon="['fab', 'github']"/></i>
        </a>
        <a href="https://www.linkedin.com/in/travisf7/">
          <i><font-awesome :icon="['fab', 'linkedin']"/></i>
        </a>
      </div>
      <p>Copyright © Travis Frazier 2019.</p>
    </div>
  </footer>
</template>


<script>
export default {
  name: "Footer",
  props: {},
  methods: {}
};
</script>

<style lang="scss" scoped>
.footer {
  width: 100%;
  background: #111;
  padding: 70px 0;
  display: flex;
  align-items: center;
  justify-content: center;
  p {
    color: #ffffffbd;
  }
  .social-links {
    z-index: 1;
    display: flex;
    width: 100%;
    justify-content: center;
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
    }
  }
}
</style>
