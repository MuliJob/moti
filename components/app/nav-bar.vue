<script setup>
const isOpen = ref(false);

function toggleMenu() {
  isOpen.value = !isOpen.value;
}

function closeMenu() {
  isOpen.value = false;
}
</script>

<template>
  <header>
    <nav class="navbar bg-base-200 backdrop-blur-md shadow-sm fixed top-0 left-0 right-0 z-50 px-4">
      <div class="flex-1">
        <NuxtLink to="/" class="btn btn-ghost text-xl">
          Moti
        </NuxtLink>
      </div>

      <div class="hidden md:flex items-center gap-3">
        <AppThemeToggle />
        <NuxtLink to="/login">
          <button class="btn btn-outline btn-primary flex items-center gap-1">
            Login
            <Icon name="ic:outline-login" size="20" />
          </button>
        </NuxtLink>
        <NuxtLink to="/register">
          <button class="btn btn-outline btn-primary flex items-center gap-1">
            Register
            <Icon name="ic:outline-person-add" size="20" />
          </button>
        </NuxtLink>
      </div>

      <div class="md:hidden">
        <button class="btn btn-ghost" @click="toggleMenu">
          <Icon :name="isOpen ? 'ic:round-close' : 'ic:round-menu'" size="28" />
        </button>
      </div>
    </nav>

    <ClientOnly>
      <div
        v-if="isOpen"
        class="md:hidden absolute top-16 right-4 w-56 bg-base-100 shadow-xl rounded-box p-4 z-50"
      >
        <div class="flex flex-col gap-3">
          <AppThemeToggle />
          <NuxtLink to="/login" @click="closeMenu">
            <button class="btn btn-outline btn-primary w-full flex items-center gap-2">
              Login
              <Icon name="ic:outline-login" size="20" />
            </button>
          </NuxtLink>
          <NuxtLink to="/register" @click="closeMenu">
            <button class="btn btn-outline btn-primary w-full flex items-center gap-2">
              Register
              <Icon name="ic:outline-person-add" size="20" />
            </button>
          </NuxtLink>
        </div>
      </div>
    </ClientOnly>
  </header>
</template>
