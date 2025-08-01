<template>
  <div class="card">
    <div class="card-title">
      <slot name="title"></slot>
    </div>
    <div class="card-content">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
};
</script>

<style scoped>
.card {
  border-radius: 12px;
  backdrop-filter: blur(10px);
  background: rgba(54, 52, 67, 0.8);
  padding: 12px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  min-width: 200px;
  box-sizing: border-box; 
  width: fit-content;
  border: 5px solid rgb(40, 40, 48);
  border: 2;
}

.card-title {
  font-size: 1.25rem;
  font-weight: bold;
  margin-bottom: 8px;
}

.card-content {
  font-size: 1rem;
}
</style>