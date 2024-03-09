<script lang="ts" setup>
function emitResponsive(v: boolean): void {
  if(v){
      const body = document.querySelector('body')
      body?.classList.remove('light-mode')
      body?.classList.add('dark-mode')
      const nav = document.getElementById('nav-respo')
      nav?.classList.remove('light-mode-nav')
      nav?.classList.add('dark-mode-nav')
      const h1 = document.getElementById('h1-respo')
      h1?.classList.remove('light-mode-nav')
      h1?.classList.add('dark-mode-nav')
      const art = document.getElementById('art')
      art?.classList.remove('light-mode-nav')
      art?.classList.add('dark-mode-nav')
      const img = document.getElementById('img')
      img?.classList.remove('light-mode-img')
      img?.classList.add('dark-mode-img')
    }
    else{
      const body = document.querySelector('body');
      body?.classList.remove('dark-mode');
      body?.classList.add('light-mode')
      const nav = document.getElementById('nav-respo')
      nav?.classList.remove('dark-mode-nav')
      nav?.classList.add('light-mode-nav')
      const h1 = document.getElementById('h1-respo')
      h1?.classList.remove('dark-mode-nav')
      h1?.classList.add('light-mode-nav')
      const art = document.getElementById('art')
      art?.classList.remove('dark-mode-nav')
      art?.classList.add('light-mode-nav')
      const img = document.getElementById('img')
      img?.classList.remove('dark-mode-img')
      img?.classList.add('light-mode-img')
    }
}
</script>
<template>
  <nav id="nav-respo">
    <span></span>
    <h1 id="h1-respo">
      Whatsapp Vittbot
    </h1>
    <SwitchMode @test-emit="emitResponsive"/>
  </nav>
</template>

<style scoped>
nav{
  width: 100%;
  display: flex;
  justify-content:space-between;
  color: var(--bg-t);
}
span{
  width: 7%;
}
</style>