<script setup lang="ts">
const technologies = [
 'SQL',
 'PostgreSQL',
 'Python',
 'Apache Spark',
 'Snowflake',
 'Pandas',
 'Excel'
]
</script>

<template>
  <section class="min-h-screen flex items-center justify-center bg-gradient-to-br from-primary-50 to-white dark:from-gray-900 dark:to-gray-800">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-32">
      <div class="text-center">
        <h1 class="...">
  Hi, I'm Gajanan
  <span class="text-primary-600">Data Engineer</span>
</h1>
        <p>
MIS Executive | Aspiring Data Engineer | 
SQL | PostgreSQL | Python | Apache Spark | Snowflake | Pandas | Excel

</p>
        <div class="flex flex-wrap justify-center gap-4 mb-12">
          <a href="#contact" class="bg-primary-600 text-white px-8 py-3 rounded-full hover:bg-primary-700 transition-colors">
            Get in Touch
          </a>
          <a href="#projects" class="border-2 border-primary-600 text-primary-600 px-8 py-3 rounded-full hover:bg-primary-50 transition-colors">
            View Projects
          </a>
        </div>
        <div class="flex flex-wrap justify-center gap-4">
          <span v-for="tech in technologies" :key="tech" class="px-4 py-2 bg-white dark:bg-gray-800 rounded-full text-sm shadow-sm">
            {{ tech }}
          </span>
        </div>
      </div>
    </div>
  </section>
</template>
