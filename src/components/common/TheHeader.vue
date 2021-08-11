<template>
  <header class="header">
    <nav class="nav container">
      <a href="#" class="logo">Logo</a>
      <ul class="nav-list" role="list">
        <li class="nav-list-item">Item</li>
      </ul>
    </nav>
  </header>
</template>



<style lang="scss" scoped>
.header {
  background: var(--surface1);
  padding: 1.5rem 0;
}
.nav {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>
