<script>
  let img = "../public/destroy_the_world_logo.png";

  function relocate_home() {
    window.location.href = "../";
  }

  function relocate_about() {
    window.location.href = "../about";
  }
</script>

<main>
  <div id="navbar" class="nav_element">
    <img src={img} id="icon" alt="icon" class="nav_element" on:click={relocate_home}/>
    <p id="about_us" class="nav_element" on:click={relocate_about}>About Us</p>
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

  #icon {
    top: 5px;
    left: 5px;
    width: 45px;
    height: 45px;
  }

  #about_us {
    left: 70%;
  }
</style>
