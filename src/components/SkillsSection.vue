<script setup lang="ts">
const skills = [
 {
  category: 'Programming & Query Languages',
  items: ['SQL', 'PostgreSQL', 'Python']
 },
 {
  category: 'Big Data & Processing',
  items: ['Apache Spark']
 },
 {
  category: 'Cloud Platform',
  items: ['AWS']
 },
 {
  category: 'Data Tools',
  items: ['Snowflake', 'Pandas', 'Excel']
 }
]
</script>

<template>
  <section id="skills" class="py-20 bg-gray-50 dark:bg-gray-900">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="section-title">Technical Skills</h2>
      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
        <div v-for="(skill, index) in skills" :key="index" class="card">
          <h3 class="text-xl font-semibold mb-4 text-primary-600">
            {{ skill.category }}
          </h3>
          <div class="flex flex-wrap gap-2">
            <span v-for="item in skill.items" :key="item"
              class="px-3 py-1 bg-primary-50 dark:bg-primary-900/20 text-primary-700 dark:text-primary-300 rounded-full text-sm">
              {{ item }}
            </span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
