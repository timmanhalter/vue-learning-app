<script setup lang="ts">
defineProps<{
  msg: string;
  links: Array<{ name: string; link: string }>;
}>();
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>Learn some things</h3>
    <nav>
      <RouterLink to="/">Learning</RouterLink>
      <!-- <RouterLink to="/about">Categories</RouterLink>|
      <RouterLink to="/about">Stack Right</RouterLink>|
      <RouterLink to="/about">Stack Wrong</RouterLink>| -->
    </nav>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
