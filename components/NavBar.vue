<template>
  <nav class="navbar is-white">
    <div class="container">
      <div class="navbar-brand">
        <a class="navbar-item brand-text" href="../">Bulma Admin</a>
        <div class="navbar-burger burger" data-target="navMenu">
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>
      <div id="navMenu" class="navbar-menu">
        <div class="navbar-start">
          <a class="navbar-item" href="admin.html">Home</a>
          <a class="navbar-item" href="admin.html">Orders</a>
          <a class="navbar-item" href="admin.html">Payments</a>
          <a class="navbar-item" href="admin.html">Exceptions</a>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  mounted() {
    const burger = document.querySelector('.burger')
    const menu = document.querySelector('#' + burger.dataset.target)
    burger.addEventListener('click', function() {
      burger.classList.toggle('is-active')
      menu.classList.toggle('is-active')
    })
  }
}
</script>

<style scoped>
nav.navbar {
  border-top: 4px solid #276cda;
  margin-bottom: 1rem;
}
.navbar-item.brand-text {
  font-weight: 300;
}
.navbar-item,
.navbar-link {
  font-size: 14px;
  font-weight: 700;
}
</style>
