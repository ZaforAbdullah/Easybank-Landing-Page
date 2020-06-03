<template>
  <div class="hello">

    <nav class="navbar">
      <img class="logo" src="../assets/images/logo.svg" alt="Logo" />
      <ul v-if="elementvisibility" class="nav-links">
          <li class="nav-item"><a href="#">Home</a></li>
          <li class="nav-item"><a href="#">About</a></li>
          <li class="nav-item"><a href="#">Blog</a></li>
          <li class="nav-item"><a href="#">Careers</a></li>
      </ul>
      <button class="firstbutton" type="button">Request Invite</button>
      
      <img v-if="elementvisibility" @click="buttontoggle" class="icon-hamburger" src="../assets/images/icon-close.svg" alt="Logo"/>
      <img v-else @click="buttontoggle" class="icon-hamburger" src="../assets/images/icon-hamburger.svg" alt="Logo"/>
      
    </nav>

    <div class="firstdiv">
      <div>
        <h1> Next generation <br> digital banking </h1>
        <p class="firstdivpara"> Take your financial life online. Your Easybank account <br> 
        will be a one-stop-shop for spending, saving, <br>
        budgeting, investing, and much more.</p>
        <button class="secondbutton" type="button">Request Invite</button>
      </div>
      <div>
        <div>
          <img class="bg-intro-desktop" src="../assets/images/bg-intro-desktop.svg" alt="Logo" />
          <img class="bg-intro-mobile" src="../assets/images/bg-intro-mobile.svg" alt="Logo" />
        </div>
        <div>
          <img class="image-mockups" src="../assets/images/image-mockups.png" alt="Logo" />
        </div>
      </div>
    </div>
    <div class="secondiv">
      <div>
        <h1> Why choose Easybank? </h1>
        <p> We leverage Open Banking to turn your bank account into your financial hub. <br>
        Control your finances like never before. </p>
      </div>
      <div class="secondivcontainer">
        <div>
          <img src="../assets/images/icon-online.svg" alt="Logo" />
          <h2> Online Banking </h2>
          <p> Our modern web and mobile applications allow you to keep track of your finances 
          wherever you are in the world. </p>

        </div>

        <div>
          <img src="../assets/images/icon-budgeting.svg" alt="Logo" />
          <h2> Simple Budgeting </h2>
          <p> See exactly where your money goes each month. Receive notifications when you’re 
          close to hitting your limits. </p>
          
        </div>

        <div>
          <img src="../assets/images/icon-onboarding.svg" alt="Logo" />
          <h2> Fast Onboarding </h2>
          <p> We don’t do branches. Open your account in minutes online and start taking control 
          of your finances right away. </p>
        </div>

        <div>
          <img src="../assets/images/icon-api.svg" alt="Logo" />
          <h2> Open API </h2>
          <p> Manage your savings, investments, pension, and much more from one account. Tracking 
          your money has never been easier. </p>          
        </div>
      </div>
     </div>
  
    <div class="thridiv">
      <h1> Latest Articles </h1>
      <div class="thirdivcontainer">
        <div> 
          <img src="../assets/images/image-currency.jpg" alt="Logo" />
          <small> By Claire Robinson </small> <br>
          <h2> Receive money in any currency with no fees </h2>
          <p> The world is getting smaller and we’re becoming more mobile. So why should you be 
          forced to only receive money in a single … </p>
         </div>
     
        <div> 
          <img src="../assets/images/image-restaurant.jpg" alt="Logo" />
          <small> By Wilson Hutton </small> <br>
          <h2> Treat yourself without worrying about money </h2>
          <p> Our simple budgeting feature allows you to separate out your spending and set 
          realistic limits each month. That means you … </p>
       </div>

        <div>
          <img src="../assets/images/image-plane.jpg" alt="Logo" />
          <small>By Wilson Hutton </small> <br>
          <h2>Take your Easybank card wherever you go </h2>
          <p> We want you to enjoy your travels. This is why we don’t charge any fees on purchases 
          while you’re abroad. We’ll even show you … </p>
          
        </div>

        <div> 
          <img src="../assets/images/image-confetti.jpg" alt="Logo" />
          <small> By Claire Robinson </small> <br>
          <h2>Our invite-only Beta accounts are now live! </h2>
          <p> After a lot of hard work by the whole team, we’re excited to launch our closed beta. 
          It’s easy to request an invite through the site ... </p>
          
       </div>

      </div>
    </div>
    <footer class="fourthidiv">
      <div>
        <img src="../assets/images/logo_white.svg" alt="Logo" /> <br> <br> <br>
        <div>
          <img class="logo" src="../assets/images/icon-facebook.svg" alt="Logo" />
          <img class="logo" src="../assets/images/icon-youtube.svg" alt="Logo" />
          <img class="logo" src="../assets/images/icon-twitter.svg" alt="Logo" />
          <img class="logo" src="../assets/images/icon-pinterest.svg" alt="Logo" />
          <img class="logo" src="../assets/images/icon-instagram.svg" alt="Logo" />
        </div>
      </div>
      <div class="footerspace0">
        About Us <br> <br>
        Contact <br> <br> 
        Blog
      </div>
      <div class="footerspace1">
        Careers <br> <br>
        Support <br> <br>
        Privacy Policy
      </div>
      <div class="footerspace2">
        <button type="button">Request Invite</button> <br> <br> <br>
        © Easybank. All Rights Reserved
      </div>
    </footer>  
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      elementvisibility : true
    }
  },
  methods: {
    buttontoggle () {
            this.elementvisibility = !this.elementvisibility;
    } 
  }
}
</script>

<style scoped>

</style>
