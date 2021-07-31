<template>
  <div>
    <div>
      <b-navbar toggleable="lg" type="dark">
        <b-navbar-brand href="#">
          <h3 class="title"><i>Kirimanjaro</i></h3>
        </b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav id="link-container" class="ml-auto">
            <b-nav-item
              target="_blank"
              href="https://kirimanjarodev.wordpress.com/about/"
            >
              <h5 class="links">About</h5>
            </b-nav-item>
            <b-nav-item><h5 class="links">Projects</h5></b-nav-item>
            <b-nav-item
              target="_blank"
              href="https://kirimanjarodev.wordpress.com/contact/"
              ><h5 class="links">Contacts</h5></b-nav-item
            >
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
  </div>
</template>

<script>
export default {
  name: 'navbar',
}
</script>

<style>
.links {
  color: rgb(253, 254, 255);
}
.links:hover {
  text-decoration-line: underline;
}
.title {
  color: rgb(253, 254, 255);
}
/* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {
}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {
}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
  .title {
    margin-left: 10px;
  }
}

/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {
  .title {
    margin-left: 20px;
  }
  #link-container {
    margin-right: 20px;
  }
}

/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {
  .title {
    margin-left: 20px;
  }
  #link-container {
    margin-right: 20px;
  }
}
</style>
