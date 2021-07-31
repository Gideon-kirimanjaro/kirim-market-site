<template>
  <div>
    <div class="content">
      <div class="content2">
        <h3 class="name">
          My name is Gideon Kirimanjaro <br />
          &nbsp;&nbsp; and this is my portfolio site
        </h3>
        <button class="projects">
          <b-link @click="projectScroll('header')" target="_blank">
            <h5 class="view">View Projects</h5>
          </b-link>
        </button>
        <h3 class="test" ref="header"></h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'info',
  methods: {
    projectScroll(refName) {
      var element = this.$refs[refName]
      var top = element.offsetTop

      window.scrollTo(0, top)
    },
  },
}
</script>

<style>
.name {
  color: white;
}
.view {
  color: white;
}
.projects {
  border-radius: 0px 10px;
  color: black;
  padding: 10px;
  background-color: rgb(131, 4, 114);
  margin-top: 30px;
}
.projects:hover {
  color: green;
}
.content {
  display: flex;
  justify-content: center;
  margin-top: 160px;
}
.test {
  margin-top: 200px;
}
/* .content2 {
  display: flex;
  justify-content: ;
} */
/* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {
  .name {
    font-size: 20px;
  }
}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {
  .projects {
    margin-left: 70px;
  }
}
/* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {
  .projects {
    margin-left: 40px;
  }
}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {
  .projects {
    margin-left: 70px;
  }
}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
  .projects {
    margin-left: 120px;
  }
}

/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {
  .projects {
    margin-left: 130px;
  }
}
</style>
