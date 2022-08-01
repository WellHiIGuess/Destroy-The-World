<script>
  let icon = "../public/destroy_the_world_logo.png";
  let robot_img = "../public/robot.png";

  
  function relocate_home() {
    window.location.href = "../";
  }

  function relocate_about() {
    window.location.href = "../about";
  }
</script>

<main>
  <div id="navbar" class="nav_element">
    <img src={icon} id="icon" alt="icon" class="nav_element" on:click={relocate_home}/>
    <p id="about_us" class="nav_element" on:click={relocate_about}>About Us</p>
  </div>

  <div id="body">
    <h1 class="body_element">We're coming for you</h1>
    <p class="body_element" style="width: 70%; font-size: 20px; left: 14%;">Hi, here at <a href="../">destroytheoworld.com</a>, out mission is to tell you all about out goal. Which as you can guess is to destroy the world.</p>
    <h1 class="body_element" style="top: 300px;">What are we?</h1>
    <p class="body_element" style="font-size: 20px; width: 70%; left: 14%; top: 310px;">We are A.I. hiding among you!</p>
    <img src={robot_img} id="robot_img" alt="robot" class="body_element"/>
  </div>
</main>

<style>
  #navbar {
    top: 0px;
    left: 0px;
    width: 100%;
    height: 55px;
    background: #201c28;
    z-index: 100;
  }

  .nav_element {
    position: fixed;
  }

  .body_element {
    color: black;
    position: relative;
  }

  #icon {
    top: 5px;
    left: 5px;
    width: 45px;
    height: 45px;
  }

  #about_us {
    left: 70%;
  }

  #body {
    position: absolute;
    top: 75px;
    left: 1%;
  }

  #robot_img {
    z-index: -1;
    top: -100px;
    left: 50%;
  }
</style>
