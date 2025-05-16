<template>
  <div class="main">
    <nav class="bg-white border-b border-gray-200 px-4 py-3 shadow-sm">
      <div class="flex justify-between items-center max-w-7xl mx-auto">
        <div class="flex items-center space-x-6">
          <!-- Logo + Titel onder elkaar -->
          <div class="flex flex-col items-start space-y-1">
            <img
                src="./media/logo.png"
                alt="House"
                class="h-10 w-auto object-contain"
                id="SmallTransform"
                ref="logo"
            />
            <h1 class="font-bold text-xl">CMS HOMEPAGE</h1>
            <p class="mt-2 font-bold">
              Week: 20
            </p>
          </div>

          <!-- Inputs -->
          <div class="flex flex-col space-y-2">
            <input type="text" class="w-40 h-8 border-1 px-2" placeholder="ET100050308🔍" />
            <input type="text" class="w-40 h-8 border-1 px-2" placeholder="#ETR-1234567" />
          </div>
        </div>


        <!-- Desktop Menu -->
        <div class="hidden md:flex space-x-6">
          <div class="flex flex-col items-center space-y-1">
            <ShoppingCartIcon class="h-15 w-15 text-gray-700" id="SmallTransform" />
            <a href="/dashboard" class="text-gray-600 hover:text-black text-sm">Bestellingen</a>
          </div>
          <div class="flex flex-col items-center space-y-1">
            <img
                src="./media/warehouse.png"
                alt="warehouse"
                class="h-15 w-15 object-contain"
                id="SmallTransform"
                ref="logo"
            />
            <a href="/pages" class="text-gray-600 hover:text-black">Magazijn</a>
          </div>
          <div class="flex flex-col items-center space-y-1">
            <UserIcon class="h-15 w-15 text-gray-700" id="SmallTransform" />
            <a href="/users" class="text-gray-600 hover:text-black">Account</a>
          </div>
        </div>
      </div>
    </nav>
    <div class="Welkom flex justify-center w-1/3 h-1/2 px-20 pb-20 mt-20 border-1 mx-auto">
      <div class="flex flex-col items-center space-y-1">
        <p class="font-bold">
          Welkom <span class="underline">Sid van Eijndhoven</span>
        </p>

        <button class="border-1 w-1/2 h-1/2 bg-gray-200">
          <a href="/users" class="text-gray-600 hover:text-black">Uitloggen</a>
        </button>
      </div>
    </div>
    <div class="flex justify-center space-x-8">
      <!-- Marketing   -->
      <div class="flex flex-col items-center space-y-1">
        <megaphone-icon class="h-15 w-15 text-gray-700 mt-20 mx-auto" id="SmallTransform"></megaphone-icon>
        <a href="/dashboard" class="text-gray-600 hover:text-black text-sm">Marketing</a>
      </div>
      <!-- Account -->
      <div class="flex flex-col items-center space-y-1">
        <UserIcon class="h-15 w-15 text-gray-700 mt-20 mx-auto" id="SmallTransform"></UserIcon>
        <a href="/dashboard" class="text-gray-600 hover:text-black text-sm">Account</a>
      </div>
      <!-- Wiki -->
      <div class="flex flex-col items-center space-y-1">
        <BookOpenIcon class="h-15 w-15 text-gray-700 mt-20 mx-auto" id="SmallTransform"></BookOpenIcon>
        <a href="/dashboard" class="text-gray-600 hover:text-black text-sm">Wiki</a>
      </div>
    </div>
    <div class="Welkom flex justify-center w-1/3 h-1/2 px-20 pb-20 mt-20 mb-20 border-1 mx-auto">
      <div class="flex flex-col items-center space-y-1">
        <p class="font-bold">
            Producten & Categoriën Administratie
          </p>
        <a href="">
          Not Shipped Overview
        </a>
        <a href="">
          Manual Stock Adjustments
        </a>
      </div>
    </div>

    </div>
</template>

<script setup>
import { ref } from 'vue'
import { ShoppingCartIcon, UserIcon, MegaphoneIcon, BookOpenIcon } from '@heroicons/vue/24/outline'

</script>
