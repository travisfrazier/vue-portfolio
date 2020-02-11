<template>
  <section class="section" id="contact">
    <div class="section-heading">
      <h2>Let's Chat</h2>
    </div>
    <p class="relocate">
      I'm currently based in San Diego, CA and I'm available for full-time work.
    </p>
    <div class="form-wrapper">
      <form method="POST" data-netlify="true">
        <div>
          <div class="input-container">
            <input
              type="text"
              name="name"
              id="name"
              required
              placeholder="Name*"
            />
          </div>
          <div class="input-container">
            <input
              type="email"
              name="email"
              id="email"
              required
              placeholder="Email*"
            />
          </div>
          <div class="input-container">
            <textarea
              id="massage"
              name="massage"
              required
              placeholder="Message*"
            />
          </div>
          <div class="button-wrapper">
            <button
              type="submit"
              class="site-btn transition-ease"
              data-wow-delay="0.2s"
            >
              Send Messege
            </button>
          </div>
          <div id="result" />
        </div>
      </form>
    </div>
    <Footer />
  </section>
</template>

<script>
import Footer from '~/components/Footer.vue';

export default {
  name: 'Contact',
  components: {
    Footer
  }
};
</script>

<style lang="scss" scoped>
.relocate {
  //text-align: center;
  margin-bottom: 3rem;
  margin-right: auto;
  margin-left: auto;
  width: 90%;
  color: #ffffffb9;
}

#contact {
  background: #424242;
}

.form-wrapper {
  //width: 55%;
  //max-width: 42rem;
  //margin: auto;
  padding-bottom: 5rem;
  @media only screen and (max-width: 600px) {
    width: 90%;
  }
}
form {
  width: 100%;
  overflow: hidden;
  label {
    display: block;
    margin-bottom: 8px;
    font-size: 1.25rem;
  }
  fieldset {
    width: 100%;
    padding: 0;
    border: none;
  }
  input,
  textarea {
    background-color: #d4d4d4;
    width: 90%;
    //display: inline;
    //border-radius: 5px;
    border: none;
    font-size: 1rem;
    height: 6rem;
    padding: 0.25rem;
    background: none;
    border: 1.25px solid black;
    border-radius: 10px;
    color: #ffffff;
  }
  input {
    height: 3.25rem;
    margin-bottom: 1rem;
  }
  .input-container {
    display: flex;
    justify-content: center;
  }
  .button-wrapper {
    display: flex;
    margin: auto;
    width: 90%;
  }
  button {
    width: 11rem;
    height: 3.25rem;
    border: none;
    border-radius: 5px;
    background-color: #ff3f80;
    color: white;
    font-size: 1.25rem;
    margin-top: 1rem;
  }
}
</style>
