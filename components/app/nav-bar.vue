<template>
  <div class="navbar bg-base-100 shadow-sm">
    <div class="flex-1">
      <NuxtLink to="/" class="btn btn-ghost text-xl">
        Moti
      </NuxtLink>
    </div>
    <div class="flex-none">
      <AppThemeToggle />
      <button class="btn btn-outline btn-primary">
        Login
        <Icon
          name="ic:outline-login"
          size="24"
        />
      </button>
    </div>
  </div>
</template>
