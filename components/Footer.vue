<script lang="ts" setup>
import Us from '/us.svg'
import Home from '/home.svg'
import Contact from '/contact.svg';
</script>
<template>
  <nav>
    <ul>
      <NuxtLink to="/About" class="us-link">
        <img :src="Us" alt="Us">
      </NuxtLink>
      <NuxtLink to="/" class="home-link">
        <img :src="Home" alt="Home" >
      </NuxtLink>
      <NuxtLink to="/Contact" class="contact-link">
        <img :src="Contact" alt="Contact">
      </NuxtLink>
    </ul>
  </nav>
</template>

<style scoped>
nav{
  width: 100%;
  height: 7vh;
  position: fixed;
  bottom: 0;
}
nav ul{
  padding: 0;
  margin: 0;
  height: 100%;
  width: 90%;
  padding: 0 5%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
nav ul a{
  display: flex;
  justify-content: center;
  text-align: center;
  width: max-content;
  padding: 0 1rem;
  transition: all ease .1s;
  border-radius: .8rem;
}
nav ul a:hover{
  background-color: #242424a1;
}/* 
nav ul a::after {
  content: 'Contact';
  position: absolute;
  bottom: 120%;
  z-index: 120;
  left: 17%;
  transform: translateX(-50%);
  background-color: #333;
  color: #fff;
  padding: .5rem .7rem;
  border-radius: 5px;
  opacity: 0;
  transition: opacity 0.3s ease;
}

nav ul a:active::after {
  opacity: 1;
}  */

.us-link::after {
  content: 'Us';
  position: absolute;
  bottom: 120%;
  z-index: 120;
  left: 17%;
  transform: translateX(-50%);
  background-color: #333;
  color: #fff;
  padding: .5rem .7rem;
  border-radius: 5px;
  opacity: 0;
  transition: opacity 0.3s ease;
}
.us-link:active::after {
  opacity: 1;
}
.home-link::after {
  content: 'Home';
  position: absolute;
  bottom: 120%;
  z-index: 120;
  left: 50%;
  transform: translateX(-50%);
  background-color: #333;
  color: #fff;
  padding: .5rem .7rem;
  border-radius: 5px;
  opacity: 0;
  transition: opacity 0.3s ease;
}
.home-link:active::after {
  opacity: 1;
}
.contact-link::after {
  content: 'Contact';
  position: absolute;
  bottom: 120%;
  z-index: 120;
  left: 83%;
  transform: translateX(-50%);
  background-color: #333;
  color: #fff;
  padding: .5rem .7rem;
  border-radius: 5px;
  opacity: 0;
  transition: opacity 0.3s ease;
}
.contact-link:active::after {
  opacity: 1;
}
</style>