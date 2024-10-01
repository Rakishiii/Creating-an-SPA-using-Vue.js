<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg bg-primary" data-bs-theme="dark">
      <div class="container-fluid">
        <img src="./assets/logo.png" alt="Logo">
        <a class="navbar-brand" href="#">Resume</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarColor01" aria-controls="navbarColor01" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarColor01">
          <ul class="navbar-nav me-auto">
          </ul>
        </div>
      </div>
    </nav>

    <main>
      <section class="resume">
        <div class="profile">
          <img :src="profileImage" class="profile-image" alt="Profile Image">
          <h2>Hi! I am Rakishi Duelle T. Dungca.</h2>
          <p>
            Student from WD-302. I am 21 years old and love to learn more about coding.
            I have different types of hobbies such as games and sports. I am currently in my
            third year and studying at Holy Angel University. My goal is to enhance my coding
            skills and learn different languages.
          </p>
        </div>

        <div class="skills">
          <h3>Skills</h3>
          <ul>
            <li>JavaScript</li>
            <li>Vue.js</li>
            <li>Sports</li>
            <li>Dancing</li>
            <li>Node.js</li>
            <li>Natural Leader</li>
          </ul>
        </div>

        <div class="education">
          <h3>Education</h3>
          <ul>
            <li>Bachelor of Science in Information Technology Web Development - Holy Angel University</li>
            <li>High School Diploma - Angeles University Foundation (2016)</li>
          </ul>
        </div>
      </section>
    </main>

    <footer class="footer">
      <p>&copy; 2024 Rakishi Duelle T. Dungca</p>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      profileImage: require('@/assets/profile.jpg'),
    };
  },
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 20px; 
  background-color: #03A89E; /* Set background color for the entire body */
  min-height: 100vh;
}

.resume {
  max-width: 600px;
  margin: 100px auto;
  border: 1px solid #ddd;
  padding: 20px;
  border-radius: 8px;
  background-color: white;  
}

.profile {
  margin-bottom: 30px;
}

img {
  width: 30px;
  height: 30px;
}

.profile-image {
  width: 150px;
  height: auto;
  border-radius: 50%;
}

h2 {
  font-size: 24px;
  color: black;     
}

h3 {
  font-size: 20px;
  margin-top: 20px;
  color:black;  
}

ul {
  list-style-type: disc;
  padding-left: 20px;
}


.footer {
  margin-top: 40px;
  text-align: center;
  background-color: #007bff;
  color: white;
  padding: 10px 0;
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
}
</style>
