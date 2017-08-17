<template>
  <div class="hello">
    <div class="header-image">
      <img src="../assets/fake_cover.png" class="cover-img">
    </div>

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
