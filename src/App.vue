<template>
  <div id="app">
    <div class="container">
      <!-- Commenting out the old JSON component -->
      <!-- <JSONComponent /> -->

      <!-- Referencing the LoginForm component -->
      <LoginForm />
    </div>
  </div>
</template>

<script>
// Importing the LoginForm component
import LoginForm from './components/LoginForm.vue'

// Commenting out the old JSON component import
// import JSONComponent from './components/JSON.vue'

export default {
  name: 'App',
  components: {
    // Commenting out the old JSON component
    // JSONComponent,
    LoginForm
  }
}
</script>

<style scoped>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex;
  justify-content: center;
  margin: 0;
  padding: 20px;
  min-height: 100vh; /* Ensure the app takes at least the full viewport height */
}

.container {
  width: 90%;
  max-width: 800px;
  margin: 0 auto;
}

.json-lab {
  width: 100%;
  margin: 20px auto;
  padding: 20px;
  background-color: #f4f4f4;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

h1,
h2 {
  color: #333;
}
h1 {
  text-align: center;
}

.lab-section {
  background-color: white;
  padding: 20px;
  margin-bottom: 20px;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.message {
  padding: 10px;
  border-radius: 5px;
  margin-top: 10px;
}

.success {
  background-color: #e7faf3;
  color: #42b883;
  border: 1px solid #42b883;
}

.highlight {
  background-color: #f0f8ff;
  font-weight: bold;
  color: #42b883;
}

code {
  background-color: #e0e0e0;
  padding: 2px 5px;
  border-radius: 4px;
  font-family: 'Courier New', Courier, monospace;
}

ul {
  list-style-type: none;
  padding: 0;
}
li {
  background-color: #f0f0f0;
  padding: 10px;
  margin: 5px 0;
  border-radius: 5px;
}
</style>
