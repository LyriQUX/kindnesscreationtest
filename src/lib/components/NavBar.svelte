<script>
  let isMenuOpen = false;

  function toggleMenu(){
    isMenuOpen = !isMenuOpen;
  }
</script>

<div class="flex items-center fixed bg-white w-full h-24 scroll-smooth shadow-lg z-10">

  <div class="flex justify-between items-center w-[100%] h-20">
    <div></div>
    <a href="/" class="w-28"><img src="/Images/TKCF - Logo.svg" class="z-50" alt="Elitespeak Logo"></a>
    <nav class:open={isMenuOpen}>
      <ul class="flex flex-col md:flex-row bg-white justify-between items-center gap-[5vh] md:gap-[2vw] py-5 mt-[0.5vh] mb-[4vh] md:m-0 font-medium text-gray-400">
        <li class="hover:text-[#243b7d] hover:underline hover:decoration-[#243b7d] ease-in duration-200"><a href="/" on:click={() => (isMenuOpen = false)}>Home</a></li>
        <li class="hover:text-[#243b7d] hover:underline hover:decoration-[#243b7d] ease-in duration-200"><a href="/#why-us" on:click={() => (isMenuOpen = false)}>About Us</a></li>
        <li class="hover:text-[#243b7d] hover:underline hover:decoration-[#243b7d] ease-in duration-200"><a href="/#team" on:click={() => (isMenuOpen = false)}>Team</a></li>
        <li class="hover:text-[#243b7d] hover:underline hover:decoration-[#243b7d] ease-in duration-200"><a href="/#services" on:click={() => (isMenuOpen = false)}>Services</a></li>
        <li class="hover:text-[#243b7d] hover:underline hover:decoration-[#243b7d] ease-in duration-200"><a href="/#reviews" on:click={() => (isMenuOpen = false)}>Reviews</a></li>
      </ul>
    </nav>
    <a href="/contact-us">
      <button class="bg-[#243b7d] lg:bg-white lg:hover:bg-[#243b7d] px-4 py-3 rounded-xl text-white lg:text-gray-400 lg:hover:text-white font-medium ease-in-out duration-500"><h3 class="text-sm">Donate Now</h3></button>
    </a>
    <button on:click={toggleMenu}>
      <img class="w-9 mr-[6vw] md:hidden" src="/Images/list.svg" alt="Menu Icon">
    </button>
  </div>

</div>