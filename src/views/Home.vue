<template>
  <div class="home">
    
    <div class="banner">
      <div class="navbar-custom">
      <nav class="custom-navigation-bar navbar navbar-light navbar-expand-md bg-faded justify-content-center">
          <a href="/" class="navbar-brand d-flex w-50 mr-auto">
            <img src="../assets/logo1.png" width="80px">
          </a>
          <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#collapsingNavbar3">
              <span class="navbar-toggler-icon"></span>
          </button>
          <div class="navbar-collapse collapse w-100" id="collapsingNavbar3">
              <ul class="nav navbar-nav ml-auto w-100 justify-content-end p-2 d-flex align-items-center">
                  <li class="nav-item">
                    <a href="" class="p-3">Home</a>
                  </li>
                  <li class="nav-item">
                    <a href="" class="p-3">Service</a>
                  </li>
                  <li class="nav-item">
                    <a href="" class="p-3">Project</a>
                  </li>
                  <li class="nav-item">
                    <a href="" class="p-3">About us</a>
                  </li>
                  <li class="nav-item">
                    <a href="" class="p-3">Contact</a>
                  </li>
                  <li>
                    <button class="btn btn-nav" type="buttom">My project</button>
                  </li>
              </ul>
          </div>
      </nav>

        
      </div>
      <div class="row">
        <div class="col-xs-6 col-sm-6 col-md-6 col-lg-6 banner-content">
          <div>
            <h1 class="head-text">creative</h1>
            <h1 class="head-text">agency</h1>
            <div class="mt-5 play-button-wrapper">
              <span><i class='fa fa-play-circle play-button' style='font-size:60px'></i></span>
              <span class="pl-2">Watch a video intro</span>
            </div>
            <div class="social-icon mt-5">
              <span><i class="fa fa-facebook-f" style="font-size:24px"></i></span>
              <span class="pl-4"><i class="fa fa-twitter" style="font-size:24px"></i></span>
              <span class="pl-4"><i class="fa fa-dribbble" style="font-size:24px"></i></span>
              <span class="pl-4"><i class="fa fa-linkedin" style="font-size:24px"></i></span>
            </div>
          </div>
        </div>
        <div class="col-xs-6 col-sm-6 col-md-6 col-lg-6 image-wrapper">
          <img src="../assets/banner.png" width="600px">
        </div>
      </div>
    </div>
  
    <!-- services -->
    <section class="service-content p-5">
      <div class="container">
        <h1 class="service-head ml-3">services & portfolio</h1>
        <div class="row service-main-contain">
          <div class="col-xs-4 col-sm-4 col-md-4 col-lg-4 d-flex mt-5" v-for="(services,index) in services" :key="index">
            <div class="services-image">
              <img :src="require('../assets/' + services.imageName)" :alt="services.name" width="50px">
            </div>
            <div class="services-contain flex-grow-1 text-left pl-3">
              <h4 class="services-name">{{services.name}}</h4>
              <p class="">{{services.tag}}</p>
            </div>
          </div>
        </div>
      </div>
      <div class="mt-5 service-image-contain">
        <section id="service-photos">
          <img src="../assets/Rectangle 20.png" alt="work">
          <img src="../assets/Rectangle 16.png" alt="work">
          <img src="../assets/image3.jpg" alt="kjb">
          <img src="../assets/Rectangle 20.png" alt="work">
        </section>
      </div>
      <div class="button">
        <button type="button" class="btn btn-border-radius p-3">VIEW ALL PROJECT</button>
      </div>
    </section>
  
    <!-- team -->
    <section class="container">
      <div class="team">
        <h2 class="team-head">Meet The Team</h2>
        <h3 class="team-subhead">greate outcome always relay on the great foundation</h3>
        <div class="row team-contain">
          <div class="col-xs-4 col-sm-4 col-md-4 col-lg-4" v-for="(person,index) in team" :key="index">
            <div class="team-image">
              <img :src="require('../assets/' + person.imageName)" :alt="person.name" width="300">
            </div>
            <div class="mt-5 team-text">
              <h4>{{person.name}}</h4>
              <p class="person-tag">{{person.tag}}</p>
              <p>
                <span><a :href="person.facebook" target="_blank">
                  <i class="fab fa-facebook icon"></i>
                  </a>
                </span>
                <span class="pl-4"><a :href="person.twitter" target="_blank">
                  <i class="fab fa-twitter icon"></i>
                  </a>
                </span>
                <span class="pl-4"><a :href="person.dribbble" target="_blank">
                  <i class="fab fa-dribbble icon"></i>
                  </a>
                </span>
                <span class="pl-4"><a :href="person.linkedIn" target="_blank">
                  <i class="fab fa-linkedin icon"></i>
                  </a>
                </span>
              </p>
            </div>
          </div>
        </div>
        <div class="button-team mt-5">
          <button type="button" class="btn btn-default p-3">LET'S CATCH ALL</button>
        </div>
      </div>
    </section>
  
    <!-- clients and achievements -->
    <section class="achievements">
      <div class="row">
        <div class="col-xs-4 col-sm-4 col-md-4 col-lg-4 achievements-image">
          <div><img src="../assets/achievement.png" width="600px"></div>
        </div>
        <div class="col-xs-8 col-sm-8 col-md-8 col-lg-8">
          <div class="achievements-contain">
            <div class="container">
            <h2 class="achievements-head">clients & achievements</h2>
            <div class="achievement-content">
              <div class="row pt-5">
                <div class="col-md-6 achievement-options">
                  <div class="row achievement-options-wrapper">
                    <div class="col-md-4"><img src="../assets/achieve4.png" width="50px"></div>
                    <div class="col-md-8 ">
                      <span class="achieve-text">emerging design agency (2017)</span>
                    </div>
                  </div>
                </div>
                <div class="col-md-6 achievement-options">
                  <div class="row">
                    <div class="col-md-4">
                      <img src="../assets/achieve4.png" width="50px"></div>
                    <div class="col-md-8">
                      <span class="achieve-text">top 10 design agency (2018)</span>
                    </div>
                  </div>
                </div>
              </div>
              <div class="row pt-5 achievement-options-wrapper">
                <div class="col-md-6 achievement-options">
                  <div class="row">
                    <div class="col-md-4">
                      <img src="../assets/achieve4.png" width="50px">
                    </div>
                    <div class="col-md-8 ">
                      <span class="achieve-text">top 5 design agency (2019) internationally </span>
                    </div>
                  </div>
                </div>
                <div class="col-md-6 achievement-options">
                  <div class="row">
                    <div class="col-md-4"><img src="../assets/achieve4.png" width="50px"></div>
                    <div class="col-md-8 t">
                      <span class="achieve-text">going to get no. 1 place internationally</span>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="company-logo">
              <img src="../assets/Trusted by the best.png" width="600px">
            </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  
    <!-- contact -->
    <section class="contact">
      <div class="container">
        <h5 class="contact-text">contact us</h5>
        <h2 class="contact-tag mt-4">Have an awesome idea in your mind? we would love to hear</h2>
        <div class="input-box mt-5">
          <span><input type="text" placeholder="enter your mail" class="email-input"></span>
          <span class="pl-4"><button type="button" class="btn btn-border-radius button-input">start</button></span>
        </div>
      </div>
    </section>
  
  
  
    <!-- footer -->
    <section class="footer">
      <div class="container pt-5">
        <div class="footer-content">
          <div class="row">
            <div class="col-xs-3 col-sm-3 col-md-3 col-lg-3">
              <img src="../assets/logo1.png" width="80px">
              <p class="agency-text pt-4">A design agency shaping ideas into products. We help startups and enterprises invent, build and launch their next project.</p>
            </div>
            <div class="col-xs-3 col-sm-3 col-md-3 col-lg-3 footer-services">
              <h5>Services</h5>
              <div class="service-text pt-3">
                <p>
                  <router-link to="/">Web Design</router-link>
                </p>
                <p>
                  <router-link to="/">App Design</router-link>
                </p>
                <p>
                  <router-link to="/">Photography</router-link>
                </p>
                <p>
                  <router-link to="/">Videography</router-link>
                </p>
              </div>
            </div>
            <div class="col-xs-3 col-sm-3 col-md-3 col-lg-3 footer-support">
              <h4 class="text-left">Support</h4>
              <div class="support-text text-left pt-3">
                <p>
                  <router-link to="/">Get Support</router-link>
                </p>
                <p>
                  <router-link to="/">Contact</router-link>
                </p>
                <p>
                  <router-link to="/">My Blog</router-link>
                </p>
                <p>
                  <router-link to="/">Privacy Policy</router-link>
                </p>
                <p>
                  <router-link to="/">Pricing</router-link>
                </p>
              </div>
            </div>
            <div class="col-xs-3 col-sm-3 col-md-3 col-lg-3 text-left footer-social">
              <h4>social</h4>
              <div class="footer-icon pt-3">
                <span><i class="fa fa-facebook" style="font-size:24px"></i></span>
                <span class="pl-4"><i class="fa fa-twitter" style="font-size:24px"></i></span>
                <span class="pl-4"><i class="fa fa-dribbble" style="font-size:24px"></i></span>
                <span class="pl-4"><i class="fa fa-linkedin" style="font-size:24px"></i></span>
              </div>
            </div>
          </div>
        </div>
        <div class="footer-bottom pt-4">
          <p> &copy;indianpix | All rights reserved 2019</p>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
  export default {
    name: 'Home',
  
  
    data() {
      return {
        services: [],
        team: [],
      }
    },
    created() {
      this.initialiseservicesData();
      this.initialiseTeamData();
    },
    methods: {
      initialiseservicesData() {
        this.services = [{
            imageName: "website-design.svg",
            name: "Web Design",
            tag: "modern web design services with new trends and direction.",
          },
          {
            imageName: "branding.svg",
            name: "Branding",
            tag: "highly professional branding and logo design work.",
          },
          {
            imageName: "motion graphics.svg",
            name: "Motion Graphics",
            tag: "modern motion graphics and animationfor business.",
          },
          {
            imageName: "ui design.svg",
            name: "ui/ux design",
            tag: "standard screen generationnd designfor all devices.",
          },
          {
            imageName: "web development.svg",
            name: "Web Development",
            tag: "website developing is something we are best in",
          },
          {
            imageName: "app testing.svg",
            name: "App testing",
            tag: "we test app for better user exprience and results",
          },
  
        ];
      },
      initialiseTeamData() {
        this.team = [{
            imageName: "man1.png",
            name: "jam potrick",
            tag: "Standard screen generation and desihn for all",
            facebook: 'https://www.facebook.com/',
            twitter: 'https://www.twitter.com/',
            dribbble: 'https://www.dribbble.com/',
            linkedIn: 'https://www.linkedin.com/',
          },
          {
            imageName: "women.png",
            name: "ema jonas",
            tag: "Standard screen generation and desihn for all",
            facebook: 'https://www.facebook.com/',
            twitter: 'https://www.twitter.com/',
            dribbble: 'https://www.dribbble.com/',
            linkedIn: 'https://www.linkedin.com/'
          },
          {
            imageName: "man1.png",
            name: "mike pens",
            tag: "Standard screen generation and desihn for all",
            facebook: 'https://www.facebook.com/',
            twitter: 'https://www.twitter.com/',
            dribbble: 'https://www.dribbble.com/',
            linkedIn: 'linkedin.com/'
          },
        ];
      },
    }
  }
</script>

<style>
.logo{
  padding-top: 5%;
}
#hamburge{
  /* display: block; */
}
  .head-text {
    color: #502EFF;
    font-size: 114px;
    font-weight: 900;
    line-height: 5rem;
    text-align: left;
  }
  
  .navbar-custom {
    position: absolute;
    width: 100%;
    z-index: 999;
  }
  
  .btn-nav {
    color: #fff;
    background: #502EFF;
    width: 150px;
    padding: 0.6rem;
    border-radius: 50px;
    line-height: 1rem;
  }
  
  .banner {
    height: 90vh;
  }
  
  .play-button-wrapper {
    display: flex;
    align-items: center;
    justify-content: left;
  }
  
  .play-button {
    color: #502EFF;
  }
  
  .image-wrapper {
    position: relative;
  }
  
  .image-wrapper img {
    position: absolute;
    right: 0;
    top: 0;
  }
  
  .banner-content {
    display: flex;
    height: inherit;
    align-items: center;
    justify-content: center;
  }
  
  .social-icon {
    display: flex;
  }
  
  .service-content {
    background: #502EFF;
  }
  
  .service-main-contain {
    padding-top: 5%;
  }
  
  .service-head {
    color: white;
    text-align: left;
    font-size: 80px;
    max-width: 34%;
  }
  
  .services-image {
    color: white;
  }
  
  .services-contain {
    color: white;
  }
  
  .services-name {
    font-size: 14px;
    font-weight: 999;
  }
  
  .service-image-contain {
    width: 98%;
    margin: auto;
  }
  
  #service-photos {
    width: 99%;
    margin: auto;
    margin-top: 10%;
    padding: 1rem;
    -webkit-column-count: 3;
    -webkit-column-gap: 0px;
    -moz-column-count: 3;
    -moz-column-gap: 0px;
    column-count: 3;
    column-gap: 15px;
  }
  
  #service-photos img {
    width: 100% !important;
    height: auto !important;
    margin-top: 1rem;
    background: #fff;
  }
  
  .btn:hover {
    color: #f53903 !important;
  }
  
  .team-head {
    color: rgb(180, 178, 175)
  }
  
  .team-subhead {
    text-align: center;
    line-height: 1.9rem;
    width: 430px;
    margin: auto;
    color: rgb(61, 61, 235);
  }
  
  .team-contain {
    margin-top: 10%;
  }
  
  .team-image {
    box-shadow: rgba(0, 0, 0, 0.2);
  }
  .person-tag{
    /* width: 200px; */
    /* padding-right: 20%; */
  }
  
  .btn-default {
    color: #fff;
    background: #502EFF;
    width: 220px;
    border-radius: 50px;
    line-height: 1.2rem;
    box-shadow: 0px 20px 30px rgba(41, 41, 41, 0.16);
  }
  
  .btn-team {
    cursor: pointer;
  }
  
  .btn-border-radius {
    color: #502EFF;
    background: #fff;
    width: 220px;
    border-radius: 50px;
    line-height: 1.2rem;
    box-shadow: 0px 20px 30px rgba(41, 41, 41, 0.16);
  }
  
  .achievements {
    margin-top: 10%;
    background-color: #FAF7FF;
  }
  
  .achievements-contain {
    padding-top: 7%;
  }
  
  .achievements-head {
    width: 600px;
    font-size: 70px;
    text-align: right;
    font-weight: 999;
    color: #502EFF;
  }
  
  .achievements-image {
    position: relative;
  }
  
  .achievements-image img {
    position: absolute;
    left: -150px;
    top: -20px;
  }
  
  .achievement-content {
    padding: 5% 30% 0 0;
    font-size: 14px;
    font-weight: 900;
  }
  
  .achieve-text {
    color: #502EFF;
    /* width: 0; */
    display: inline-block;
    text-align: left;
  }
  
  .contact-text{
    color: rgb(180, 178, 175);
  }
  .contact-tag {
    text-align: center;
    line-height: 1.9rem;
    width: 550px;
    margin: auto;
  }
  
  .company-logo {
    display: flex;
    align-items: left;
    padding: 8% 0 8% 0;
  }
  
  .email-input {
    border: solid 3px;
    border-radius: 50px;
    padding: 0.5rem;
    width: 25%;
    font-size: 16px;
    color: rgb(61, 61, 235);
    ;
  }
  
  .button-input {
    background-color: rgb(61, 61, 235);
    font-size: 24px;
    color: #fff;
    padding: 0.5rem;
    width: 150px;
    box-shadow: 0px 20px 30px rgba(41, 41, 41, 0.16)
  }
  
  .footer {
    background-color: #FAF7FF;
  }
  
  .footer-content {
    color: #676767;
    border-top: 1px solid #CBD5F9;
    border-bottom: 1px solid #CBD5F9;
    padding: 10% 0 10% 0;
  }
  
  .footer-bottom {
    text-align: center;
    color: blue;
    padding: 1% 0 3% 0;
  }
  
  .agency-text {
    text-align: left;
    padding-left: 35%;
    padding-top: 5%;
    color: #502EFF;
  }
  
  .service-text a {
    color: #502EFF;
  }
  
  .support-text {
    line-height: 0.8rem;
    color: #502EFF;
  }
  
  .support-text a {
    color: #502EFF;
  }
  
  .footer-icon i {
    color: #502EFF;
  }
  
  .custom-navigation-bar {
    width: 80%;
    margin: auto;
  }
  
  .container {
    margin-top: 10%;
  }

/* mobile-view */

@media only screen and (max-width: 600px){
  
  .play-button-wrapper,.social-icon,.head-text {
    display: inline-flex;
    text-align: center;
  }
  .custom-navigation-bar {
    width: 100%;
    margin: auto;
  }
  #collapsingNavbar3 {
    background: #fff;
  }
  .service-content {
    width:100%;
    padding:1rem 0 1rem 0  !important;
  }
  
  .head-text{
    font-size: 80px;
  }
  .image-wrapper img{
    display: none;
  }
  .service-head{
    font-size: 50px;
    margin: 0;
    text-align: center;
    max-width: 100%;
  }
  #service-photos{
    padding: 0;
  }
  .achievement-options-wrapper {
    padding: 0 !important;
    width: 100%;
  }
  .achievement-options {
    margin-top: 2rem;
  }
  .button{
    padding-top: 20%
  }
  .btn:hover {
    color: #f53903 !important;
  }
  .team-subhead{
    width: 340px;
    font-size: 26px;
  }
  .team-image{
    padding-top: 10%;
  }
  .achievements-head{
    width: 350px;
    font-size: 50px;
    text-align: center;
  }
  .contact-tag{
    width: 340px;
    font-size: 20px;
  }
  .email-input{
    width: 200px;
  }
  .button-input{
    padding: 12px;
    width: 90px;
  }
  .agency-text{
    text-align: center;
    padding-left: 7%;
  }
  #nav-options{
    display: none !important;  
  }
  .achievements-image {
     display: none !important;  
  }
  .achievements-head{
    width: 330px;
  }
  .achievement-content{
    padding: 0;
  }
  .achieve-text{
    text-align: center;
    width: 100%;
  }
  .footer-content {
    text-align: left;
  }
  .agency-text {
    padding:0;
    text-align:left;
  }
  .footer-services {
    margin-top: 2rem;
  }
  .footer-support {
    margin-top: 2rem;
  }
  .footer-social {
    margin-top: 2rem;
  }
}
</style>

