<script setup lang="ts">
const projects = [
 {
  title: 'Olist E-commerce SQL Analysis',
  description: 'Performed in-depth analysis on Brazilian e-commerce dataset using advanced SQL queries to derive business insights.',
  tech: ['SQL', 'PostgreSQL'],
  link: 'https://github.com/gajananjadhav-ai'
 }
]
</script>

<template>
  <section id="projects" class="py-20 bg-white dark:bg-gray-800">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="section-title">Featured Projects</h2>
      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
        <div v-for="(project, index) in projects" :key="index" 
          class="card hover:translate-y-[-4px] transition-transform">
          <h3 class="text-xl font-semibold mb-3">{{ project.title }}</h3>
          <p class="text-gray-600 dark:text-gray-300 mb-4">
            {{ project.description }}
          </p>
          <div class="flex flex-wrap gap-2 mb-4">
            <span v-for="tech in project.technologies" :key="tech"
              class="px-2 py-1 bg-gray-100 dark:bg-gray-700 rounded text-sm">
              {{ tech }}
            </span>
          </div>
          <p class="text-primary-600 font-medium">
            {{ project.metrics }}
          </p>
        </div>
      </div>
    </div>
  </section>
</template>
