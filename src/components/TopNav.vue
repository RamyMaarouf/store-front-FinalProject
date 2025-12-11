<template>
  <nav>
    <div class="logo">
      <a href="/">
        <img src="/bestbuy-logo.png" alt="Best Buy Logo"> 
      </a>
    </div>
    </nav>
</template>

<script>
export default {
  name: 'TopNav',
  // You can define props, data, or methods here if necessary
}
</script>

<style scoped>
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  /* FIXED: Best Buy Blue background */
  background-color: #004694; 
  color: #fff;
  padding-top: 0.5rem;
  padding-left: 1rem;
  padding-right: 1rem;
  padding-bottom: 0.25rem;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1000;
}

.logo img {
    height: 40px; /* Adjust height as necessary for your logo */
    vertical-align: middle;
}

/* If you need styles for links, dropdowns, etc., add them here */

/* Example link style */
nav a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

nav a:hover {
    color: #FFC600; /* Best Buy Yellow */
}
</style>