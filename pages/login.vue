<template>
  <div class="max-w-sm mx-auto bg-base-200 p-6 rounded-box shadow-md">
    <form class="space-y-4">
      <fieldset>
        <legend class="text-xl font-semibold text-center mb-4">
          Login
        </legend>

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

        <div class="flex items-center justify-between text-sm mt-2">
          <label class="flex items-center gap-2 cursor-pointer">
            <input type="checkbox" class="checkbox checkbox-sm">
            <span class="label-text">Remember me</span>
          </label>
          <a href="#" class="link link-hover text-primary">Forgot password?</a>
        </div>

        <button type="submit" class="btn btn-primary w-full mt-4">
          Login
        </button>
      </fieldset>
    </form>

    <!-- Divider -->
    <div class="divider my-6">
      Or
    </div>

    <!-- Social login buttons -->
    <div class="flex flex-col gap-3">
      <button class="btn btn-outline w-full flex items-center justify-center">
        <img
          src="https://www.svgrepo.com/show/475656/google-color.svg"
          class="w-5 h-5 mr-2"
          alt="Google"
        >
        Continue with Google
      </button>
      <button class="btn btn-outline w-full flex items-center justify-center">
        <img
          src="https://www.svgrepo.com/show/475654/github-color.svg"
          class="w-5 h-5 mr-2"
          alt="GitHub"
        >
        Continue with GitHub
      </button>
    </div>

    <!-- Register link -->
    <p class="text-center text-sm text-gray-600 mt-6">
      Don't have an account?
      <a href="/register" class="text-primary font-semibold hover:underline">
        Register here
      </a>
    </p>
  </div>
</template>
