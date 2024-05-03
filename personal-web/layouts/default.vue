<script setup lang="ts">
const route = useRoute()

const links = [{
  label: 'Profile',
  avatar: {
    src: 'https://avatars.githubusercontent.com/u/66852892?v=4'
  },
  to: '/'
}, {
  label: 'Resume',
  icon: 'i-heroicons-document-text',
  to: `/resume`
}, {
  label: 'Contact Info',
  icon: 'i-heroicons-user-circle',
  to: '/components/command-palette'
}, {
  label: 'Projects',
  icon: 'i-heroicons-rectangle-stack',
  to: '/components/command-palette'
}]
</script>

<template>
  <UHorizontalNavigation :links="links" class="border-b border-gray-200 dark:border-gray-800" />
</template>
