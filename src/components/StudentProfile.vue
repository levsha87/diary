<template>
    <div class="student-profile">
      <img :src="student.photo || '/src/assets/no-profile-image.svg'" alt="Profile Picture" class="profile-pic"/>
      <h2>{{ student.name }}</h2>
      <p>Class: {{ student.class }}</p>
      <p>Email: {{ student.email }}</p>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  
  const student = ref({
      name: 'John Doe',
      class: '12A',
      email: 'john.doe@example.com',
      photo: ''
  })
  </script>
  
  <style scoped>
  .student-profile {
    display: flex;
    flex-direction: column;
    align-items: start;
    border: 1px solid #ccc;
    padding: 10px;
    border-radius: 8px;
    margin: 20px;
  }
  
  .profile-pic {
    width: 60px;
    height: 60px;
    border-radius: 50%;
    margin-right: 15px;
  }
  </style>