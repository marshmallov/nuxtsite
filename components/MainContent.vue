<template>
    <div class="parallax-container">
      <section id="home-section">
        <div
          class="parallax-item"
          style="background-image: url('/images/IMG_1.jpg')"
        >
          <div class="parallax-content">
            <div class="content-card">
              <h1>Ovonel</h1>
              <p>
                <!-- Add your content here -->
              </p>
            </div>
          </div>
        </div>
      </section>
      
      <section id="about-section">
        <div
          class="parallax-item"
          style="background-image: url('/images/IMG_2.jpg')"
        >
          <div class="parallax-content">
            <div class="content-card">
              <p>
                We create 
              </p>
            </div>
          </div>
        </div>
      </section>
      
      <section id="services-section">
        <div
          class="parallax-item"
          style="background-image: url('/images/IMG_3.jpg')"
        >
          <div class="parallax-content">
            <div class="content-card">
              <div class="text-white">
                <!-- Content here -->
                 <p>
                    We Travel
                 </p>
              </div>
            </div>
          </div>
        </div>
      </section>
      
      <section id="contact-section">
        <div
          class="parallax-item"
          style="background-image: url('/images/IMG_4.jpg')"
        >
          <div class="parallax-content">
            <div class="content-card">
              <p>
                <!-- Your contact section content -->
                 We Like IT
              </p>
            </div>
          </div>
        </div>
      </section>
    </div>
  </template>
  
  <script>
  export default {
    name: "MainContent",
    data() {
      return {
        State: {
          isPlaying: false
        }
      };
    },
    methods: {
      // Your methods here
    }
  };
  </script>
  
  <style >

  
  .parallax-container {
    display: flex;
    flex-direction: column;
  }
  
  .parallax-item {
    position: relative;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
  }
  
  
  .parallax-content {
    position: relative;
    z-index: 1;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .content-card {
    background-color: rgba(255, 255, 255, 0); /* Transparency for the content card */
    padding: 2rem;
    border-radius: 8px;
    max-width: 600px;
    text-align: center;
  }
  
  h1 {
    font-size: 10rem;
    margin-bottom: 1rem;
    color: #ffffff;
  }
  
  h2 {
    font-size: 1.5rem;
    margin-bottom: 1rem;
    color: #ffffff;
  }
  
  p {
    color: #ffffff;
  }
  </style>
  