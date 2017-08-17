<template>
  <div class="hello">
    <b-navbar toggleable type="light" variant="info" toggle-breakpoint="md">

      <b-nav-toggle target="nav_collapse"></b-nav-toggle>

      <b-navbar-brand href="#">NavBar</b-navbar-brand>

      <b-collapse is-nav id="nav_collapse">

        <b-nav is-nav-bar>
          <b-nav-item href="#">Link</b-nav-item>
          <b-nav-item href="#" disabled>Disabled</b-nav-item>
        </b-nav>

        <!-- Right alignd nav items -->
        <b-nav is-nav-bar class="ml-auto">

          <b-nav-form>
            <b-form-input size="sm" class="mr-sm-2" type="text" placeholder="Search"/>
            <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
          </b-nav-form>

          <b-nav-item-dropdown text="Lang" right>
            <b-dropdown-item to="#">EN</b-dropdown-item>
            <b-dropdown-item to="#">ES</b-dropdown-item>
            <b-dropdown-item to="#">RU</b-dropdown-item>
            <b-dropdown-item to="#">FA</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown right>
            <!-- Using button-content slot -->
            <template slot="button-content">
              <em>User</em>
            </template>
            <b-dropdown-item to="#">Profile</b-dropdown-item>
            <b-dropdown-item to="#">Signout</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-nav>

      </b-collapse>
    </b-navbar>

    <b-jumbotron header="ThruDerm" lead="Over the counter Transdermal Topical Analgesics" >
      <p>Have Muscle Pain?</p>
      <b-btn variant="primary" href="#">Contact Us</b-btn>
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
          <p> Please contact kasdkfljasdlkfjalskdfjlksdjf</p>
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

</style>
