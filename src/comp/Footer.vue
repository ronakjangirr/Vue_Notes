<template>
  <div>
    <v-card >

      <v-row >
        <v-col cols="8" class="primary pa-10">

          <div class="d-flex justify-space-around flex-wrap ">
            <div class=" bg-blue">
              <h5>Section</h5>
              <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Features</a></li>
                <li><a href="#">Pricing</a></li>
                <li><a href="#">FAQs</a></li>
                <li><a href="#">About</a></li>
              </ul>
            </div>

            <div>
              <h5>Section</h5>
              <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Features</a></li>
                <li><a href="#">Pricing</a></li>
                <li><a href="#">FAQs</a></li>
                <li><a href="#">About</a></li>
              </ul>
            </div>

            <div>
              <h5>Section</h5>
              <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Features</a></li>
                <li><a href="#">Pricing</a></li>
                <li><a href="#">FAQs</a></li>
                <li><a href="#">About</a></li>
              </ul>
            </div>

            <div>
              <h5>Section</h5>
              <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Features</a></li>
                <li><a href="#">Pricing</a></li>
                <li><a href="#">FAQs</a></li>
                <li><a href="#">About</a></li>
              </ul>
            </div>


          </div>
        </v-col>

        <v-col cols="4" >
          <form class="d-flex flex-wrap pa-5">
            <h2 class="primary--text">LET'S STAY IN TOUCH</h2>
            <p>Be the first to know about special promotions, new collections and more when you sign up for our emails!
            </p>
            <div>
              <input type="email" placeholder="Your Email" /><span><v-btn depressed color="primary">
                  Submit
                </v-btn></span>

            </div>
          </form>
        </v-col>

      </v-row>

    </v-card>


  </div>
</template>

<script>

export default {
  name: "FooterVue",
}

</script>

<style scoped>
ul {
  list-style-type: none;
  color: aliceblue;
}

a {
  text-decoration: none;
  color: aliceblue;
}

li a {
  color: aliceblue;
}
</style>