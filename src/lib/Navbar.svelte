<script lang="ts">
  import Button from './Button.svelte';
  
  let isMenuOpen = false;
</script>

<nav class="fixed top-0 left-0 right-0 z-50 bg-cream/90 backdrop-blur-sm border-b border-gray-200/50">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex justify-between items-center h-20">
      <!-- Logo -->
      <div class="flex-shrink-0 flex items-center">
        <a href="/" class="flex items-center gap-2">
          <!-- Brckt Logo Icon -->
          <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect width="32" height="32" rx="6" fill="#191817"/>
            <path d="M8 10 L8 22 M8 10 L14 10 C16 10 17 11 17 13 C17 15 16 16 14 16 L8 16 M8 16 L15 16 C17 16 18 17 18 19 C18 21 17 22 15 22 L8 22" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
            <path d="M20 10 L20 22 M20 16 L24 10 M20 16 L24 22" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
          <span class="font-bold text-xl tracking-tight">Brckt</span>
        </a>
      </div>

      <!-- Desktop Navigation -->
      <div class="hidden md:flex items-center space-x-8">
        <a href="#how-it-works" class="text-sm font-medium hover:text-primary-brand transition-colors">How It Works</a>
        <a href="#features" class="text-sm font-medium hover:text-primary-brand transition-colors">Features</a>
        <a href="#tournaments" class="text-sm font-medium hover:text-primary-brand transition-colors">Tournaments</a>
      </div>

      <!-- Right Side -->
      <div class="hidden md:flex items-center space-x-6">
        <a href="https://app.brckt.io" class="text-sm font-medium hover:text-primary-brand transition-colors">Login</a>
        <Button href="https://app.brckt.io/group/create" className="!py-2 !px-4 !text-sm">Create Bracket &rarr;</Button>
      </div>

      <!-- Mobile menu button -->
      <div class="md:hidden flex items-center">
        <button on:click={() => isMenuOpen = !isMenuOpen} class="text-gray-600 hover:text-gray-900 focus:outline-none">
          <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
        </button>
      </div>
    </div>
  </div>
</nav>
