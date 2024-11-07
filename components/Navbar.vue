<template>
    <nav class="">
      <div class=" ">
        <div class="">
          <ul  class="">
            <li>
              <a href="#home-section" @click.prevent="scrollToSection('home-section')" class="text-white">Ovonel</a>
            </li>
            <li>
              <a href="#about-section" @click.prevent="scrollToSection('about-section')" class="text-white">Create</a>
            </li>
            <li>
              <a href="#services-section" @click.prevent="scrollToSection('services-section')" class="text-white">Travel</a>
            </li>
            <li>
              <a href="#contact-section" @click.prevent="scrollToSection('contact-section')" class="text-white">Like It</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </template>
  
  <script>
 

  export default {
    
    name: "Navbar",
    components: {
  
    },
    setup(){
      return {
   // Expose the State so you can access isPlaying in your template
      };
    },
    data() {
      return {
        audio: null,
        audioSources: [
        ],
        currentAudioIndex: 0,
      };
    },
    methods: {
      scrollToSection(sectionId) {
        const element = document.getElementById(sectionId);
        const yOffset = -30; // Adjust this value to match the height of your navbar
        const y =
          element.getBoundingClientRect().top + window.pageYOffset + yOffset;
        window.scrollTo({ top: y, behavior: "smooth" });
        
      },
    },
    
  };
  </script>
  
  <style >
  nav {
    background-color: #000000;
    padding: 1rem;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
    margin: 0
  }
  ul {
    list-style: none;
    display: flex;
    gap: 1rem;
  }
  li {
    display: inline;
  }
  a {
    color: white;
    text-decoration: none;
  }
  a:hover {
    text-decoration: underline;
  }
  
  </style>
  