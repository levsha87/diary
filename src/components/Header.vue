<template>
    <header class="header">
      <img src="/src/assets/logo.svg" alt="School Diary Logo" class="logo" />
      <nav>
        <ul>
          <li><router-link to="/">Home</router-link></li>
          <li><router-link to="/profile">Student Profile</router-link></li>
          <!-- You can add more links here as needed -->
        </ul>
      </nav>
    </header>
  </template>
  
  <script setup>
  // No script needed for now, but you can add reactive properties or methods here if needed
  </script>
  
  <style scoped lang="less">
  @base-bg-color: #343a40;
@base-link-color: white;
@box-shadow-color: rgba(0, 0, 0, 0.5);
@link-margin: 20px;

.header {
  background-color: @base-bg-color;
  color: @base-link-color;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem;
  box-shadow: 0 2px 4px @box-shadow-color;

  .logo {
    height: 50px;
  }

  nav {
    ul {
      list-style-type: none;
      margin: 0;
      padding: 0;
      display: flex;

      li {
        margin-left: @link-margin;
        
        a {
          color: @base-link-color;
          text-decoration: none;

          &:hover {
            text-decoration: underline;
          }
        }
      }
    }
  }
}
  </style>