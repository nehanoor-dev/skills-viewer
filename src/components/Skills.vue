<template>
    <section id="skills" class="text-center py-5" style=" border-radius: 8px; padding: 50px;">
      <h2 style="font-family: 'Roboto', sans-serif; font-size: 2.5rem; margin-bottom: 20px;">Skills</h2>
      <v-container>
        <v-row>
          <v-col v-for="skill in skills" :key="skill.name" cols="12" md="4">
            <v-card class="mx-auto" style="width: 90%; transition: transform 0.3s;">
              <v-card-title>
                <v-icon style="font-size: 48px; color: #00796b;">{{ skill.icon }}</v-icon>
                <span class="font" style="font-size: 1.5rem; color: #333;">{{ skill.name }}</span>
              </v-card-title>
              <v-card-text style="font-size: 1.1rem; color: #555;">{{ skill.description }}</v-card-text>
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
        skills: [
          {
            name: 'Vue.js',
            icon: 'mdi-vuejs',
            description: 'Progressive JavaScript framework for building UIs.'
          },
          {
            name: 'React',
            icon: 'mdi-react',
            description: 'A JavaScript library for building user interfaces.'
          },
          {
            name: 'Node.js',
            icon: 'mdi-nodejs',
            description: 'JavaScript runtime built on Chrome\'s V8 engine.'
          },
          {
            name: 'Express.js',
            icon: 'mdi-nodejs',
            description: 'Fast, unopinionated, minimalist web framework for Node.js.'
          },
          {
            name: 'MongoDB',
            icon: 'mdi-database',
            description: 'NoSQL database for modern applications.'
          },
          {
            name: 'Vuex',
            icon: 'mdi-vuex',
            description: 'State management library for Vue.js applications.'
          },
          {
            name: 'Pinia',
            icon: 'mdi-state-machine',
            description: 'Next generation state management for Vue.'
          },
          {
            name: 'Redux',
            icon: 'mdi-redux',
            description: 'Predictable state container for JavaScript apps.'
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
  
  .v-icon {
    font-size: 48px; /* Increased icon size */
    color: #00796b; /* Consistent icon color */
    margin-right: 10px;
  }
  .font {
    color: aliceblue;
  }
  </style>
  