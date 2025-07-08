<script setup lang="ts">
</script>

<template>
  <div class="relative pt-16">
    <!-- Hero Section -->
    <div class="hero bg-base-200 min-h-screen">
      <div class="hero-content flex-col lg:flex-row-reverse">
        <img
          src="https://s.alicdn.com/@sc04/kf/Hb57aa11ae16340c2a2134dbed854590bK.jpg_300x300.jpg"
          class="max-w-sm rounded-lg shadow-2xl"
        >
        <div>
          <h1 class="text-5xl font-bold">
            Buy & Sell Auto Spare Parts with Moti
          </h1>
          <p class="py-6">
            Find quality spare parts for all vehicle makes and models — or list your own! Whether you're a car owner, mechanic, or reseller, our platform connects you to the right parts at the right price.
          </p>
          <button class="btn btn-outline btn-primary">
            Get Started
          </button>
        </div>
      </div>
    </div>

    <!-- Shop Now Section -->
    <div class="mt-12 px-4">
      <h2 class="text-4xl font-bold mb-6 text-center">
        Shop Now
      </h2>

      <div class="overflow-x-auto scrollbar-hide">
        <div class="flex gap-6 whitespace-nowrap">
          <!-- Card Component -->
          <div v-for="i in 8" :key="i" class="card bg-base-100 w-72 shadow-md inline-block">
            <figure>
              <img
                src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
                alt="Spare Part"
              >
            </figure>
            <div class="card-body">
              <h2 class="card-title">
                Spare Part {{ i }}
              </h2>
              <p>Durable and reliable part for your vehicle.</p>
              <div class="card-actions justify-end">
                <button class="btn btn-primary">
                  Buy Now
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
