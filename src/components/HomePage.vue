<template>
    <div class="home">
      <h1>{{ welcomeMessage }}</h1>
      <p>This is your digital diary to track and plan all your school activities efficiently.</p>
      <div class="features">
        <div class="feature">
          <h3>📅 Daily Schedules</h3>
          <p>Keep track of your daily classes and assignments.</p>
        </div>
        <div class="feature">
          <h3>📚 Homework Tracking</h3>
          <p>Never miss a deadline with easy homework tracking.</p>
        </div>
        <div class="feature">
          <h3>📝 Exams and Tests</h3>
          <p>Prepare for exams with schedules and reminders.</p>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  
  const welcomeMessage = ref('Welcome to Your School Diary');
  </script>
  
  <style scoped>
  .home {
    display: flex;
    flex-direction: column;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
    text-align: center;
  }
  
  .logo {
    max-width: 150px;
    margin: 20px;
  }
  
  .features {
    display: flex;
    justify-content: space-around;
    margin-top: 40px;
    width: 100%;
  }
  
  .feature {
    flex: 1;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 15px rgba(0,0,0,0.1);
  }
  
  @media (max-width: 768px) {
    .features {
      flex-direction: column;
    }
  
    .feature {
      margin-bottom: 20px;
      text-align: center;
    }
  }
  </style>