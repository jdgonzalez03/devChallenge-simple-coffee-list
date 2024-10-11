<template>
  <article class="item">
    <img
      src="https://csyxkpbavpcrhwqhcpyy.supabase.co/storage/v1/object/public/assets/coffee-challenge/cappuccino.jpg"
      alt="Cappuccino"
    />
    <span class="popular">Popular</span>
    <aside class="description-container">
      <h2 class="title-item">Cappuccino</h2>
      <p class="price">$5.20</p>
    </aside>
    <aside class="container-rating">
      <ul>
        <li>
          <img src="/src/assets/resources/Star_fill.svg" alt="Star rating" />
        </li>
        <li>5.0</li>
        <li class="votes">(65 votes)</li>
      </ul>
      <p class="sold-out">Sold out</p>
    </aside>
  </article>
</template>

<style scoped>
.item {
  position: relative;
}

.container-rating {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

.container-rating ul {
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 4px;
  font-size: var(--font-size-price);
  font-weight: bold;
}

.votes {
  color: var(--color-text-votes);
}

.popular {
  position: absolute;
  top: 3%;
  left: 3%;
  padding: 4px 12px;
  border: none;
  border-radius: 32px;
  font-size: var(--font-size-small-text);
  font-weight: bold;
  color: var(--background-color-body);
  background-color: var(--color-text-label-popular);
}

.description-container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

.price {
  background-color: var(--background-color-price-label);
  font-size: var(--font-size-price);
  font-weight: bold;
  color: var(--background-color-body);
  padding: 4px 8px;
  border: none;
  border-radius: 4px;
}

.title-item {
  font-size: var(--font-size-body);
}

.sold-out {
  font-size: var(--font-size-price);
  font-weight: bold;
  color: var(--color-text-sold-out);
}
</style>
