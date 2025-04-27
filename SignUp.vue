<template>
    <div class="flex min-h-screen">
      <!-- Left: Form Section -->
      <div class="w-full md:w-1/2 flex flex-col justify-center items-center bg-white px-8 py-12">
        <div class="w-full max-w-md">
          <p class="text-sm text-gray-500 mb-2 text-center">Step 01 of 03</p>
          <h1 class="text-3xl font-bold text-green-700 mb-2 text-center">GET STARTED NOW!</h1>
          <p class="text-gray-500 mb-6 text-center">Please enter your details.</p>
          <form @submit.prevent>
            <div class="mb-4">
              <label class="block text-gray-700 font-semibold mb-1">Name</label>
              <input type="text" placeholder="Enter your name" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-green-400" />
            </div>
            <div class="mb-4">
              <label class="block text-gray-700 font-semibold mb-1">Email</label>
              <input type="email" placeholder="Enter your email" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-green-400" />
            </div>
            <div class="mb-6">
              <label class="block text-gray-700 font-semibold mb-1">Password</label>
              <input type="password" placeholder="********" class="w-full px-4 py-2 border rounded focus:outline-none focus:ring-2 focus:ring-green-400" />
            </div>
            <button type="submit" class="w-full bg-green-700 text-white py-2 rounded font-semibold hover:bg-green-800 transition mb-4">
              Sign up
            </button>
          </form>
          <button class="w-full flex items-center justify-center border py-2 rounded mb-4 hover:bg-gray-100 transition">
            <img src="https://www.svgrepo.com/show/355037/google.svg" alt="Google" class="w-6 h-6 mr-2" />
            <span>Sign in with Google</span>
          </button>
          <p class="text-center text-gray-600">
            Have an account?
            <a href="#" class="text-green-700 font-semibold hover:underline">Sign in</a>
          </p>
        </div>
      </div>
      <!-- Right: Image Section -->
      <div class="hidden md:block w-1/2 relative">
        <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=800&q=80"
             alt="Elderly people smiling"
             class="w-full h-full object-cover opacity-80" />
        <!-- Logo Overlay -->
        <div class="absolute top-8 right-8 flex flex-col items-end">
          <svg width="40" height="40" viewBox="0 0 24 24" fill="none" class="mb-2">
            <path d="M12 2C13.1046 2 14 2.89543 14 4V12C14 13.1046 13.1046 14 12 14C10.8954 14 10 13.1046 10 12V4C10 2.89543 10.8954 2 12 2Z" fill="#FBBF24"/>
            <path d="M12 22C16.4183 22 20 18.4183 20 14H4C4 18.4183 7.58172 22 12 22Z" fill="#FBBF24"/>
          </svg>
          <span class="text-black text-2xl font-bold leading-tight text-right">Golden<br>Connect</span>
        </div>
      </div>
    </div>
  </template>
  
  <script setup>
  // No script logic needed for static UI
  </script>