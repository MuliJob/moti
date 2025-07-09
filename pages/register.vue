<template>
  <div class="max-w-3xl mx-auto bg-base-200 p-8 rounded-2xl shadow-xl">
    <form class="space-y-6">
      <fieldset>
        <legend class="text-2xl font-bold text-center mb-6">
          Register, it's free!
        </legend>

        <!-- Two-column form layout -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
          <div>
            <label class="label" for="username">
              <span class="label-text">Username</span>
            </label>
            <input
              id="username"
              type="text"
              class="input input-bordered w-full"
              placeholder="Enter your username"
              required
            >
          </div>

          <div>
            <label class="label" for="email">
              <span class="label-text">Email</span>
            </label>
            <input
              id="email"
              type="email"
              class="input input-bordered w-full"
              placeholder="Enter your email"
              required
            >
          </div>

          <div>
            <label class="label" for="password">
              <span class="label-text">Password</span>
            </label>
            <input
              id="password"
              type="password"
              class="input input-bordered w-full"
              placeholder="Enter your password"
              required
              minlength="6"
            >
          </div>

          <div>
            <label class="label" for="confirm-password">
              <span class="label-text">Confirm Password</span>
            </label>
            <input
              id="confirm-password"
              type="password"
              class="input input-bordered w-full"
              placeholder="Confirm your password"
              required
              minlength="6"
            >
          </div>
        </div>

        <!-- Submit Button -->
        <div class="mt-6">
          <button type="submit" class="btn btn-primary w-full text-lg">
            Let's go!
          </button>
        </div>
      </fieldset>
    </form>

    <!-- Divider -->
    <div class="divider my-8 text-sm text-gray-500">
      Or
    </div>

    <!-- Social login buttons -->
    <div class="flex flex-col gap-4">
      <button class="btn btn-outline w-full flex items-center justify-center">
        <img src="https://www.svgrepo.com/show/475656/google-color.svg" class="w-5 h-5 mr-2" alt="Google">
        Continue with Google
      </button>
      <button class="btn btn-outline w-full flex items-center justify-center">
        <img src="https://www.svgrepo.com/show/475654/github-color.svg" class="w-5 h-5 mr-2" alt="GitHub">
        Continue with GitHub
      </button>
    </div>

    <!-- Already have an account link -->
    <p class="text-center text-sm text-gray-600 mt-6">
      Already have an account?
      <a href="/login" class="text-primary font-semibold hover:underline">
        Log in here
      </a>
    </p>
  </div>
</template>
