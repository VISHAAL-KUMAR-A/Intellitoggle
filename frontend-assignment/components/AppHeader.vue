<template>
  <header style="position: sticky; top: 0; z-index: 50; width: 100%; background-color: #42389E; margin: 0; padding: 0;">
    <div style="min-height: 60px; display: flex; align-items: center; justify-content: space-between; padding: 0 1rem; position: relative;">
      <!-- Logo -->
      <img 
        src="/Light Monochrome.png" 
        alt="IntelliToggle Logo" 
        style="width: 80px; height: 48px; object-fit: contain; filter: drop-shadow(0 0 4px rgba(255,255,255,0.3));"
      />
      
      <!-- Navigation Items - Centered -->
      <nav style="position: absolute; left: 50%; transform: translateX(-50%); display: flex; align-items: center; gap: 1.5rem; top: 50%; transform: translate(-50%, -30%);">
        <a 
          href="#" 
          class="nav-item nav-home"
        >
          Home
        </a>
        <a 
          href="#" 
          class="nav-item nav-about"
        >
          About
        </a>
        <a 
          href="#" 
          class="nav-item nav-pricing"
        >
          Pricing
        </a>
      </nav>
      
      <!-- Empty div to balance the layout -->
      <div style="width: 80px;"></div>
    </div>
  </header>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@300;700&display=swap');

.nav-item {
  font-family: 'DM Sans', sans-serif;
  font-size: 12px;
  line-height: 100%;
  letter-spacing: 0%;
  text-align: center;
  text-decoration: none;
  color: white;
  transition: opacity 0.2s ease;
}

.nav-item:hover {
  opacity: 0.8;
}

.nav-home {
  font-weight: 700;
  width: 58px;
  height: 26px;
}

.nav-about {
  font-weight: 300;
  width: 57px;
  height: 26px;
}

.nav-pricing {
  font-weight: 300;
  width: 62px;
  height: 26px;
}

/* Desktop styles */
@media (min-width: 768px) {
  .nav-item {
    font-size: 14px;
  }
  
  .nav-home {
    width: 40px;
  }
  
  .nav-about {
    width: 39px;
  }
  
  .nav-pricing {
    width: 43px;
  }
  
  header div {
    padding: 0 2.5rem !important;
  }
  
  header img {
    width: 120px !important;
    height: 65px !important;
  }
  
  nav {
    gap: 1.5rem !important;
  }
}

/* Mobile responsive adjustments */
@media (max-width: 767px) {
  .nav-item {
    font-size: 14px;
    padding: 4px 8px;
  }
  
  .nav-home {
    width: auto;
    min-width: 40px;
  }
  
  .nav-about {
    width: auto;
    min-width: 40px;
  }
  
  .nav-pricing {
    width: auto;
    min-width: 40px;
  }
  
  nav {
    gap: 0.75rem !important;
  }
}
</style>
