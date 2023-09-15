<script setup lang="ts">
import Card from '../components/Card.vue'
</script>

<template>
  <main>
    <ul role="list" className='card-list'>
      <Card href="https://docs.fleek.xyz/" title="Fleek Documentation"
        body="Learn about Fleek & the available services by cheking our official docs.">
        <img height="31" width="31" src="@/assets/fleekMark.svg" />
      </Card>

      <Card href="https://vuejs.org/guide/introduction.html" title="Vue Documentation" body="Learn about Vue in their official docs.">
        <img height="31" width="31" src="@/assets/logo.svg" />
      </Card>

      <Card href="https://blog.fleek.xyz/" title="Fleek Blog" body="Checkout our Blog for more information about Fleek.">
        <img height="31" width="31" src="@/assets/fleekMark.svg" />
      </Card>

      <Card href="https://vitejs.dev/guide/" title="Vite Documentation"
        body="Learn about Vite & how it can bring you a modern development experience.">
        <img height="31" width="31" src="@/assets/vite.svg" />
      </Card>
    </ul>
  </main>
</template>

<style scoped>
.card-list {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 15px;
}

main {
  width: 75%;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0 auto;
  gap: 2.5rem;
}

</style>
