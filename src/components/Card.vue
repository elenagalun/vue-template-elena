<script setup lang="ts">
const props = defineProps<{
  title: string;
  body: string;
  href: string;
}>()

function getUrl() {
  return props.href;
}
</script>

<template>
  <li className='card'>
    <a :href="getUrl()">
      <div className='card-top-row'>
        <slot />
        <h2>
          {{ title }}
        </h2>
      </div>
      <p>
        {{ body }}
      </p>
    </a>
  </li>
</template>

<style scoped>
.card {
  list-style: none;
}

.card>a {
  color: white;
  box-sizing: border-box;
  height: 100%;
  display: flex;
  flex-direction: column;
  text-decoration: none;
  border-radius: 1.5rem;
  border: 0.85px solid #313538;
  gap: 15px;
  padding: 2rem 1.25rem;
}

.card-top-row {
  gap: 15px;
  display: flex;
  align-items: start;
}

.card h2 {
  font-size: 1.25rem;
  line-height: 2rem;
  font-weight: 700;
  margin: 0;
  color: white;
}

.card p {
  text-align: start;
  font-size: 16px;
  line-height: 1.5rem;
  color: #9ca3af;
  margin: 0;
}
</style>
