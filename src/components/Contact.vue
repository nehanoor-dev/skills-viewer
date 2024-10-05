<template>
    <section id="contact" class="text-center py-5">
      <h2 style="font-family: 'Roboto', sans-serif; font-size: 2.5rem; margin-bottom: 20px; color: #333;">Contact Me</h2>
      <v-container>
        <v-form @submit.prevent="sendMessage" class="contact-form">
          <v-text-field
            v-model="name"
            label="Your Name"
            required
            outlined
            class="my-3"
          ></v-text-field>
          <v-text-field
            v-model="email"
            label="Your Email"
            required
            type="email"
            outlined
            class="my-3"
          ></v-text-field>
          <v-textarea
            v-model="message"
            label="Your Message"
            required
            outlined
            class="my-3"
          ></v-textarea>
          <v-btn type="submit" color="primary" class="send-btn my-4">Send</v-btn>
        </v-form>
      </v-container>
    </section>
  </template>
  
  <script>
  export default {
    data() {
      return {
        name: '',
        email: '',
        message: ''
      };
    },
    methods: {
      sendMessage() {
        alert(`Message sent from ${this.name}!`);
      }
    }
  }
  </script>
  
  <style>
  .contact-form {
    max-width: 400px;
    margin: auto;
    padding: 20px;
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  }
  
  .v-text-field, .v-textarea {
    border-radius: 8px;
  }
  
  .send-btn {
    transition: background-color 0.3s, transform 0.2s;
  }
  
  .send-btn:hover {
    background-color: #1976d2;
    color: white;
    transform: translateY(-2px);
  }
  </style>
  