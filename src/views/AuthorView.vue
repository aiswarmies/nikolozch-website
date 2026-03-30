<template>
  <div class="author-template">
    <div class="gh-outer">
      <header class="author-header">
        <h1 class="author-name">Nikoloz</h1>
        <p class="author-bio">Tech writeups, thoughts and ideas</p>
      </header>

      <div class="post-feed">
        <article v-for="post in posts" :key="post.slug" class="post-card">
          <div class="post-card-content">
            <a class="post-card-content-link" :href="`/${post.slug}/`">
              <header class="post-card-header">
                <span class="post-card-tags">{{ post.tag }}</span>
                <h2 class="post-card-title">{{ post.title }}</h2>
              </header>
              <section class="post-card-excerpt">
                <p>{{ post.excerpt }}</p>
              </section>
            </a>
            <footer class="post-card-meta">
              <time class="post-card-meta-date" :datetime="post.date">{{ post.dateFormatted }}</time>
              <span class="post-card-meta-length">{{ post.readTime }}</span>
            </footer>
          </div>
        </article>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { useRoute } from 'vue-router'

const route = useRoute()

const posts = ref([
  {
    slug: 'devvortex-hack-the-box',
    title: 'Devvortex',
    tag: 'Hack The Box',
    image: 'devvortex.png',
    excerpt: 'Easy difficulty Linux machine with a Vue.js website that leaks internal API endpoints...',
    date: '2024-01-15',
    dateFormatted: 'January 15, 2024',
    readTime: '5 min read'
  },
  {
    slug: 'exatlon-hack-the-box',
    title: 'Exatlon',
    tag: 'Hack The Box',
    image: 'exatlon.png',
    excerpt: 'Hard difficulty Linux machine...',
    date: '2024-02-20',
    dateFormatted: 'February 20, 2024',
    readTime: '8 min read'
  },
  {
    slug: 'lovetok-hack-the-box',
    title: 'LoveTok',
    tag: 'Hack The Box',
    image: 'lovetok.png',
    excerpt: 'Easy difficulty machine...',
    date: '2024-03-10',
    dateFormatted: 'March 10, 2024',
    readTime: '4 min read'
  },
  {
    slug: 'monitored-hack-the-box',
    title: 'Monitored',
    tag: 'Hack The Box',
    image: 'monitored.png',
    excerpt: 'Medium difficulty Linux machine with Nagios monitoring...',
    date: '2024-04-05',
    dateFormatted: 'April 5, 2024',
    readTime: '7 min read'
  }
])
</script>
