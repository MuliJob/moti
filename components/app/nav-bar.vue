<template>
  <div class="navbar bg-base-500 backdrop-blur-md shadow-sm fixed top-0 left-0 right-0 z-50">
    <div class="flex-1">
      <NuxtLink to="/" class="btn btn-ghost text-xl">
        Moti
      </NuxtLink>
    </div>
    <div class="flex-none">
      <AppThemeToggle />
      <NuxtLink to="/login">
        <button class="btn btn-outline btn-primary">
          Login
          <Icon name="ic:outline-login" size="24" />
        </button>
      </NuxtLink>
    </div>
  </div>
</template>
