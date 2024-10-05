<template>
    <section id="projects" class="text-center py-5" style=" border-radius: 8px; padding: 50px; box-shadow: 0 4px 20px rgba(0, 0, 0, 0.15);">
      <h2 style="font-family: 'Roboto', sans-serif; font-size: 2.5rem; margin-bottom: 20px;">Projects</h2>
      <v-container>
        <v-row>
          <v-col v-for="project in projects" :key="project.title" cols="12" md="6">
            <v-card class="mx-auto" style="width: 90%; transition: transform 0.3s; overflow: hidden;">
              <v-img :src="project.image" height="200" class="transition-fade" cover></v-img>
              <v-card-title class="font" style="font-size: 1.5rem;  font-weight: bold;">{{ project.title }}</v-card-title>
              <v-card-text style="font-size: 1.1rem; color: #555;">{{ project.description }}</v-card-text>
              <v-card-actions>
                <v-btn :href="project.link" target="_blank" color="primary" class="transition-fade">View Project</v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </section>
  </template>
  
  <script>
  export default {
    data() {
      return {
        projects: [
          {
            title: 'Portfolio Website',
            description: 'A personal portfolio website to showcase my skills and projects.',
            image: 'https://i0.wp.com/curiositygym.com/wp-content/uploads/2022/05/portfolio1.jpg?fit=1920%2C1080&ssl=1',
            link: 'https://example.com'
          },
          {
            title: 'E-commerce App',
            description: 'A fully functional e-commerce application built with React and Node.js.',
            image: 'https://marketingreport.one/Article%20Images/Key%20Industy%20Images/e_commerce_Marketing_Report.jpg',
            link: 'https://example.com'
          },
          {
            title: 'Chat Application',
            description: 'Real-time chat application using Vue.js and Firebase.',
            image: 'https://www.chanty.com/blog/wp-content/uploads/2021/07/Team-Chat-Apps-740x380.png',
            link: 'https://example.com'
          },
          {
            title: 'Task Manager',
            description: 'A task management application built with Vue and Express.js.',
            image: 'https://miro.medium.com/v2/resize:fit:720/format:webp/1*8G1vA7egoxrL4Bb7RAgnPQ.jpeg',
            link: 'https://example.com'
          },
        ]
      };
    }
  }
  </script>
  
  <style>
  .v-card {
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
    border-radius: 8px;
    margin-top: 20px;
    transition: transform 0.3s;
  }
  
  .v-card:hover {
    transform: translateY(-5px);
  }
  
  .v-img {
    border-radius: 8px 8px 0 0;
    transition: transform 0.5s ease;
  }
  
  .v-btn {
    transition: background-color 0.3s;
  }
  .font {
    color: aliceblue;
  }
  
  .v-btn:hover {
    background-color: #1976d2;
    color: white;
  }
  </style>
  