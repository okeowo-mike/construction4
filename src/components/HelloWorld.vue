<template>
  <!-- <div class="hello"> -->
    <div class="hero">
      <video autoplay loop muted playsinline class="hero-video">
        <source src="../assets/hero-video-3.mp4" type="video/mp4" />
        Your browser does not support the video tag.
      </video>
      <div class="hero-content">
        <h1>WELCOME TO MY CONSTRUCTION SITE</h1>
        <p class="hero-text-1">Some captivating text about your amazing product or service</p>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus exercitationem libero
          doloribus neque.
        </p>
        <button class="hero-learn-btn">Learn More</button>
      </div>
    </div>
    <!-- <h1>{{ msg }}</h1>
    <p>
      For a guide and recipes on how to configure / customize this project,<br />
      check out the
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener">vue-cli documentation</a>.
    </p>
    <h3>Installed CLI Plugins</h3>
    <ul>
      <li>
        <a
          href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-babel"
          target="_blank"
          rel="noopener"
          >babel</a
        >
      </li>
      <li>
        <a
          href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint"
          target="_blank"
          rel="noopener"
          >eslint</a
        >
      </li>
    </ul>
    <h3>Essential Links</h3>
    <ul>
      <li><a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">Forum</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">Twitter</a></li>
      <li><a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a></li>
    </ul>
    <h3>Ecosystem</h3>
    <ul>
      <li><a href="https://router.vuejs.org" target="_blank" rel="noopener">vue-router</a></li>
      <li><a href="https://vuex.vuejs.org" target="_blank" rel="noopener">vuex</a></li>
      <li>
        <a href="https://github.com/vuejs/vue-devtools#vue-devtools" target="_blank" rel="noopener"
          >vue-devtools</a
        >
      </li>
      <li><a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener">vue-loader</a></li>
      <li>
        <a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener"
          >awesome-vue</a
        >
      </li>
    </ul> -->
  <!-- </div> -->
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* ///////////////////////////////// */
/* This is the KEY part - make it cover the screen! */
.hero {
  margin-top: -5.5rem;
  position: relative; /* Needed for absolute positioning of video and content */
  width: 100%;
  height: 100vh; /* Use viewport height to fill the screen */
  overflow: hidden; /* Hide any overflow from the video */
}

.hero-video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover; /* Crucial:  Makes the video fill the container */
  z-index: 0; /* Keep the video behind the content */
}

.hero-content {
  position: relative;
  z-index: 1; /* Bring the text to the front */
  color: white; /* Adjust text color as needed */
  text-align: center; /* Center the text */
  padding: 20px; /* Add some padding */
  margin-top: 7rem;
}

h1 {
  font-size: 3.5em;
  margin-bottom: 10px;
}

p {
  font-family: "Times New Roman", Times, serif;
  font-size: 1.2rem;
  font-weight: 100;
  max-width: 700px;
  margin: auto;
  text-align: center;
}

.hero-text-1 {
  padding-top: 0.5rem;
}

.hero-learn-btn {
  margin-top: 4rem;
  width: 200px;
  height: 50px;
  border-radius: 15px;
  background-color: transparent;
  border: 1.5px #d8d300 solid;
  color: white;
  font-size: 23px;
  font-family: 'Times New Roman', Times, serif;
  font-weight: lighter;
letter-spacing: 1px;
}
</style>
