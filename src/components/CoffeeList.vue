<script setup>
import ItemCoffee from '@/components/ItemCoffee.vue'
</script>

<template>
  <main>
    <img class="img-vector" src="/src/assets/resources/vector.svg" alt="Vector" />
    <h1 class="heading">Our Collection</h1>
    <p class="body-text">
      Introducing our Coffee Collection, a selection of unique coffees <br />
      from different roast types and origins, expertly roasted in small <br />batches and shipped
      fresh weekly.
    </p>
    <ul class="filters">
      <li>
        <button>All Products</button>
      </li>

      <li>
        <button>Available Now</button>
      </li>
    </ul>

    <section class="list">
      <ItemCoffee />
    </section>
  </main>
</template>

<style scoped>
main {
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  gap: 2rem;
  width: 100%;
  max-width: 950px;
  height: 100%;
  margin: 60px auto 0;
  padding: 0;
  background-color: var(--background-color-list);
  border-radius: 16px;
}

.img-vector {
  position: absolute;
  top: 8%;
  left: 50%;
}

/*Texts & buttons*/
.heading {
  margin-top: 80px;
  font-size: var(--font-size-heading);
  text-align: center;
  z-index: 1;
}

.body-text {
  font-size: var(--font-size-body);
  color: var(--color-text-votes);
  font-weight: 600;
  text-align: center;
  z-index: 1;
}

.filters {
  font-family: var(--font-family);
  list-style: none;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  gap: 16px;
}

.filters button {
  font-size: var(--font-size-label);
  font-weight: 600;
  color: var(--color-text-content);
  background-color: transparent;
  border: 1px solid transparent;

  border-radius: 8px;
  padding: 8px 16px;
  cursor: pointer;
  transition: all 0.3s ease;
}

.filters button:hover {
  border: 1px solid var(--color-text-votes);
  background-color: var(--color-text-votes);

  transform: translateY(-2px);
}
</style>
