<template>
    <v-app-bar app color="#1E88E5" dark>
      <v-toolbar-title>Neha Noor</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn text to="#about">About</v-btn>
      <v-btn text to="#skills">Skills</v-btn>
      <v-btn text to="#projects">Projects</v-btn>
      <v-btn text to="#contact">Contact</v-btn>
    </v-app-bar>
  </template>
  
  <style>
  .v-btn {
    transition: color 0.3s;
  }
  
  .v-btn:hover {
    color: #FFD700; /* Gold color on hover */
  }
  </style>
  