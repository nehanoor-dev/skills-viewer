<template>
    <section id="about" class="text-center py-5" style=" border-radius: 8px; padding: 50px; box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);">
      <h2 style="font-family: 'Roboto', sans-serif; font-size: 2.5rem; margin-bottom: 20px;">About Me</h2>
      <v-container>
        <v-row>
          <v-col cols="12" md="6" class="d-flex align-center">
            <v-card class="mx-auto" style="width: 90%; transition: transform 0.3s;">
              <v-img
                src="https://images.playground.com/95a9fc96aec64f86b05b63ab86dcc39d.jpeg"
                height="200px"
                class="rounded-top"
                cover
              ></v-img>
              <v-card-text>
                <p style="font-size: 1.1rem; color: #555;">
                  I am a passionate JavaScript developer with expertise in <strong>Vue.js</strong>, <strong>React</strong>, and <strong>Node.js</strong>. I love building interactive web applications and continuously improving my skills.
                </p>
              </v-card-text>
            </v-card>
          </v-col>
          
          <v-col cols="12" md="6" class="d-flex align-center">
            <v-card class="mx-auto" style="width: 90%; transition: transform 0.3s;">
              <v-img
                src="https://img.freepik.com/free-photo/celebration-labour-day-with-3d-cartoon-portrait-working-woman_23-2151306618.jpg?t=st=1726908516~exp=1726912116~hmac=4beef8fbf222712c0767191869ac01ea1a8056156771f05046a6e87ac6a9c5f9&w=826"
                height="200px"
                class="rounded-top"
                cover
              ></v-img>
              <v-card-text>
                <h3 style="font-family: 'Roboto', sans-serif; color: #00796b;">My Journey</h3>
                <p style="font-size: 1.1rem; color: #555;">
                  With a strong foundation in both front-end and back-end development, I focus on creating seamless user experiences while optimizing performance. My goal is to contribute to meaningful projects that make a difference.
                </p>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
  
        <v-row class="mt-4">
          <v-col class="d-flex align-center">
            <v-card class="mx-auto" style="width: 90%; transition: transform 0.3s;">
              <v-img
                src="https://cdn.mos.cms.futurecdn.net/x8oyLJtDJBPmL59WUoa36C-1200-80.jpg"
                height="200px"
                class="rounded-top"
                cover
              ></v-img>
              <v-card-text>
                <h3 style="font-family: 'Roboto', sans-serif; color: #00796b;">Hobbies & Interests</h3>
                <p style="font-size: 1.1rem; color: #555;">
                  In my free time, I enjoy exploring new technologies, contributing to open-source projects, and staying updated with industry trends. I believe in continuous learning and personal growth.
                </p>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </section>
  </template> /** ye html ky liye ha..mtlab sturcture bnany ky liye */
  
  <style>   /** Ye css ha  */
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
  }
  </style>
  