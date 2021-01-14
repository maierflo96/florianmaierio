<template>
  <div class="page-container">

    <md-app style="min-height: 100vh;">

      <md-app-toolbar style="background-color:grey">


        <span class="md-title" style="color: aliceblue" >
          <a style="color: aquamarine">f</a>lorian<a style="color: aquamarine">m</a>aier.<a style="color: orangered">io</a><a class="blinking">|</a></span>


        <img src="../assets/logo.png" class="logo"/>

      </md-app-toolbar>
    <md-app-content>
      <div style="padding-top:20px">
      <h1>Design.</h1>
      <h1 style="color:orangered">Code.</h1>
      <h1>Passion.</h1>
    </div>
    <div>
      <md-divider></md-divider>
        <div class="md-layout md-gutter md-alignment-center" style="padding-top: 30px">
          <div class="md-layout-item md-medium-size-75 md-small-size-50 md-xsmall-size-100" style="padding-top:40px;margin-left:40px">
          <h2> I'm a software developer based in Vienna, Austria. I have been working as a Java and JavaScript developer for a few major companies. For work I have been programming Java Spring Applications, as well as both Front- and Backend NodeJs Applications.
            I also love creating iOS apps using Swift and SwiftUi. But that's not all, because what I love most, is attempting new challenges and finding new problems to solve. Eagerly waiting for all the problems out there needing to be solved.
          </h2>
          </div>
          <div class="md-layout-item md-medium-size-15 md-small-size-50 md-xsmall-size-100" >
            <img style=max-height:430px  src="../assets/BearWithURL.png" />
          </div>
        </div>
      <div class="md-layout md-gutter md-alignment-center" style="padding-top: 40px;padding-bottom: 40px">
        <div class="md-layout-item md-medium-size-33 md-small-size-50 md-xsmall-size-100">

          <a href="#" class="fa fa-linkedin" @click="open('http://linkedin.com/in/florian-maier')"></a>


      </div>
        <div class="md-layout-item md-medium-size-33 md-small-size-50 md-xsmall-size-100">

          <a href="#" class="fa fa-envelope" @click="open('mailto:florian@florianmaier.io')"></a>

        </div>

        <div class="md-layout-item md-medium-size-33 md-small-size-50 md-xsmall-size-100">

        <a href="#" class="fa fa-github" @click="open('https://github.com/maierflo96')"></a>

        </div>

      </div>
      </div>
      <md-divider/>
    <div class="md-layout md-gutter md-alignment-top-center list">
      <div class="md-layout-item md-layout md-gutter md-alignment-center  md-size-10 md-small-hide">
      </div>
      <div class="md-layout-item md-layout md-gutter md-alignment-center  md-size-45 md-small-size-100">

      <div class="md-layout-item md-size-85 md-small-size-65">
    <h1 style="text-align: left">What I Love</h1>
      </div>

        <div class="md-layout-item md-size-85 md-small-size-65">
      <h3> &lt;/&gt; Front End Programming </h3>
        </div>
        <div class="md-layout-item md-size-85 md-small-size-65">

      <h3> &lt;/&gt; Back End Programming </h3>
        </div>
        <div class="md-layout-item md-size-85 md-small-size-65">

          <h3> &lt;/&gt; Java </h3>
        </div>

        <div class="md-layout-item md-size-85 md-small-size-65" >

      <h3> &lt;/&gt; Project Management </h3>
        </div>

          <div class="md-layout-item md-size-85 md-small-size-65">
      <h3> &lt;/&gt; UI/UX Design</h3>
          </div>

            <div class="md-layout-item md-size-85 md-small-size-65">
      <h3> &lt;/&gt; Firebase</h3>
            </div>

      </div>

    <div class="md-layout-item md-layout md-gutter md-alignment-center md-size-45 md-small-size-100">
      <div class="md-layout-item md-size-85 md-small-size-65">
        <h1 style="text-align: left">Projects</h1>
      </div>

      <div class="md-layout-item md-size-85 md-small-size-65">
        <h3> &lt;/&gt; Coming Soon... </h3>
      </div>


    </div>
    </div>


  <div class="footer">

  <h3 @click="open('https://github.com/maierflo96/florianmaierio')">View this page on GitHub</h3>
  </div>
    </md-app-content>

    </md-app>

  </div>
</template>

<script>
export default {
  name: 'Page',
  methods: {
    open: function (url) {
      window.open(url, "_blank");
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
md-app {

  min-height: 100vh;

}

.page-container{
  min-height: 100vh;
}
.md-title {
  font-family: monaco,Consolas,Lucida Console,monospace;
}
h1 {
  font-family: monaco,Consolas,Lucida Console,monospace;
  line-height: 1;
}
h2 {
  font-family: monaco,Consolas,Lucida Console,monospace;
  line-height: 1.8;
}
.fa {
  padding: 10px;
  font-size: 40px;
  text-align: center;
  text-decoration: none;
  margin: 2px 2px;
  border-radius: 100%;
}
.fa-linkedin {
  background: #007bb5;
  color: white !important;
}
.fa-github {
  background: #007bb5;
  color: white !important;
}
.fa-envelope {
  background: orangered;
  color: white !important;
}
.list{
  padding-top: 40px;
  padding-bottom: 80px;
  text-align: left;
  font-family: monaco,Consolas,Lucida Console,monospace;
}
.blinking {
  -webkit-animation: blinking 2s infinite;
  animation: blinking 2s infinite;
}
.footer{

  padding-bottom: 5px;
  padding-left: 30px;
  background-color:grey;
  color: aliceblue;
  text-align:left;
position: absolute;
  bottom: 0;
  left:0;
  width: 100%;
}
.logo{
max-height:50px;
  position: absolute;
  right:0;
  padding-right:30px
}

@keyframes blinking {
  0% {
    color: transparent;
  }
  49% {
    color: transparent
  }
  50% {
    color: yellow;
  }
}
</style>
