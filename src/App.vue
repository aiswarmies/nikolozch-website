<template>
  <div id="app" class="viewport">
    <header class="gh-head outer">
      <div class="gh-head-inner inner">
        <div class="gh-head-brand">
          <router-link to="/" class="gh-head-logo">
            Nikostan
          </router-link>
          <button class="gh-search gh-icon-btn" aria-label="Search this site">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" width="20" height="20">
              <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"></path>
            </svg>
          </button>
          <button class="gh-burger" aria-label="Main Menu"></button>
        </div>
        <nav class="gh-head-menu">
          <ul class="nav">
            <li class="nav-home" :class="{ 'nav-current': $route.path === '/' }">
              <router-link to="/">Home</router-link>
            </li>
            <li class="nav-about" :class="{ 'nav-current': $route.path === '/about' }">
              <router-link to="/about">About</router-link>
            </li>
            <li class="nav-posts">
              <router-link to="/author/nikoloz">Posts</router-link>
            </li>
          </ul>
        </nav>
      </div>
    </header>

    <main class="site-main outer">
      <div class="inner">
        <router-view />
      </div>
    </main>

    <footer class="site-footer outer">
      <div class="inner">
        <section class="copyright">
          <a href="/">Nikostan</a> &copy; 2026 All rights reserved.
        </section>
        <nav class="site-footer-nav">
          <router-link to="/">Home</router-link>
          <router-link to="/about">About</router-link>
          <a href="/rss/">RSS</a>
        </nav>
      </div>
    </footer>
  </div>
</template>

<script setup>
</script>

<style scoped>
</style>
