<template>
    <section class="hero">
      <v-img
        src="https://your-background-image-url.jpg"
        height="400"
        class="d-flex align-center justify-center"
      >
        <div class="overlay">
          <h1>Welcome to My Portfolio</h1>
          <h2>Neha Noor</h2>
          <p>Full Stack Developer</p>
          <p>Crafting solutions, one line of code at a time.</p>
        </div>
      </v-img>
    </section>
  </template>
  
  <style>
  .hero {
    position: relative;
  }
  
  .overlay {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: white;
    text-align: center;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7);
  }
  
  h1, h2 {
    transition: transform 0.5s;
  }
  
  .hero:hover h1 {
    transform: scale(1.1);
  }
  </style>
  