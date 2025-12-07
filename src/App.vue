<template>
  <footer>
    <p>&copy; 2025 Best Buy Cloud-Native App. All rights reserved.</p>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      products: [],
      cartItems: [],
      cartCount: 0 
    };
  },
  methods: {
    fetchProducts() {
        // Your existing product fetching logic
    },
    // FIX: Removed parameter name entirely to resolve ESlint's 'no-unused-vars' error.
    addToCart() { 
        // Your existing add to cart logic
    }
  },
  created() {
      // Your existing created hook logic
  }
}
</script>
<style>
/* 2. BODY: REMOVE GRASS/IMAGE BACKGROUND for a clean look */
body {
  /* background-image: url('@/assets/bby-background.jpg'); */
  /* background-size: cover; */
  /* background-position: center; */
  /* background-attachment: fixed; */
  background-color: #f7f7f7; /* Light gray background for a modern look */
  margin: 0;
  padding: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 100px; 
  padding-bottom: 50px;
}

/* 3. HEADER & NAVIGATION: BEST BUY BLUE */
header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  background-color: #004694; /* Best Buy Blue */
  padding: 0 20px;
  z-index: 1000;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.header-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
}

.logo-title {
  display: flex;
  align-items: center;
}

.logo {
  height: 40px; 
  margin-right: 15px;
}

.title {
  color: white;
  font-size: 1.5rem;
  margin: 0;
}

nav ul {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
}

nav li {
  margin-left: 20px;
}

nav a {
  color: #fff;
  text-decoration: none;
  font-weight: bold;
}

nav a:hover {
  color: #FFC600; /* Best Buy Yellow on hover */
}

/* 4. FOOTER: BEST BUY BLUE */
footer {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: #004694; /* Best Buy Blue */
  color: #fff;
  padding: 0.5rem;
  margin: 0;
  z-index: 999;
}

/* 5. BUTTONS: BEST BUY YELLOW */
button {
  padding: 10px;
  background-color: #FFC600; /* Best Buy Yellow */
  color: #000; 
  border: none;
  border-radius: 5px;
  cursor: pointer;
  height: 42px;
  font-weight: bold;
  transition: background-color 0.2s;
}

.product-controls button:hover, .checkout-button:hover {
  background-color: #002D59; /* A darker Best Buy Blue/Navy for hover contrast */
  color: white;
}

/* You can keep or adjust your existing product-card styles here */
.product-card {
  /* ... */
}
</style>