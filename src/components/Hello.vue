<template>
  <div class="hello">
    <b-navbar toggleable type="light" variant="info" toggle-breakpoint="md" class="bg-info">

      <b-nav-toggle target="nav_collapse"></b-nav-toggle>

      <b-navbar-brand href="#"><img src="../assets/thruderm.png" class="logo-icon"></b-navbar-brand>

      <b-collapse is-nav id="nav_collapse">

        <b-nav is-nav-bar>
        </b-nav>

        <!-- Right alignd nav items -->
        <b-nav is-nav-bar class="ml-auto">

          <b-nav-form>
            <b-nav-item href="#home" disabled>Home</b-nav-item>
            <b-nav-item href="#store" disabled>Store</b-nav-item>
            <b-nav-item href="#contact" disabled>Contact</b-nav-item>
          </b-nav-form>

        </b-nav>

      </b-collapse>
    </b-navbar>

    <b-jumbotron header="ThruDerm" lead="Over the counter Transdermal Topical Analgesics" class="jumbotron">
      <p>Have Muscle Pain?</p>
      <b-btn variant="primary" href="#contact">Contact Us</b-btn>
    </b-jumbotron>


<!--
    <div class="header-image">
      <img src="../assets/fake_cover.png" class="cover-img">
    </div>
-->

    <h1>{{ msg }}</h1>

    <!--What is it?-->
    <div class="about-container">
      <div class="flex-container">
        <div class="about-icon">
          <img src="../assets/medical.svg">
        </div>
        <div>
          <h2> What is ThruDerm?</h2>
        </div>
        <div>
          <ul>
            <li>
              A Transdermal ointment for sustained localized pain relief and inflammation reduction
            </li>
            <li>
              Patented Penetrating Pain Relief
            </li>
            <li>
              Accelerated Healing Action
            </li>
          </ul>
        </div>
      </div>

    </div>


    <!--Contact-->
    <div class="contact-container" id="contact">
      <div class="flex-container">
        <div class="contact-icon">
          <img src="../assets/contact.svg">
        </div>
        <div>
          <h2> Contact </h2>
        </div>
        <div>
          <b-form>
            <b-label for="firstName">First Name</b-label>
            <b-form-input id="firstName">
            </b-form-input>
            <b-label for="lastName">Last Name</b-label>
            <b-form-input id="lastName">
            </b-form-input>
            <b-label for="companyName">Company</b-label>
            <b-form-input id="companyName">
            </b-form-input>
            <b-label for="message">Message</b-label>
            <b-form-input id="message">
            </b-form-input>
            <b-form-fieldset
              id="fieldset1"
              description="Let us know your name."
              label="Enter your name"
              :feedback="feedback"
              :state="state"
            >
              <b-form-input id="input1" :invalid="invalid" v-model="name"></b-form-input>
            </b-form-fieldset>
            <b-button>Submit</b-button>
          </b-form>
        </div>
      </div>

    </div>


  </div>
</template>

<script>
  export default {
    name: 'hello',
    data() {
      return {
        msg: 'Over the counter Transdermal Topical Analgesics',
      };
    },
  };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1, h2 {
    font-weight: normal;
  }

  h2 {
    border-bottom: solid #158F98;

  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: block;
    margin: 0 10px;
    color: #474D4E;
  }

  a {
    color: #474D4E;
  }

  .header-image {

  }
  .cover-img {
    height: 600px;
    width: 100%;
  }
  .about-icon {
    height: 200px;
    width: 200px;
  }

  .contact-icon {
    height: 200px;
    width: 200px;
  }

  .flex-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin-bottom: 40px;
  }
  .bg-info {
    background-color: #E8E9EB !important;
  }
  .jumbotron {
    background: url('../assets/temp_cover2.jpg') no-repeat fixed center;
    opacity: 50%;
  }

</style>
