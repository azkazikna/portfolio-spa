<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <!-- <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header> -->

  <header
        class="fixed top-0 w-full flex justify-center transition duration-300 ease-linear z-[99] bgVal bg-blackval dark:bg-background dark:bg-opacity-70 dark:backdrop-blur-sm backdrop-blur-sm border-b-[0.2px]  border-textLight dark:border-white border-opacity-20 dark:border-opacity-20">
        <div class="container flex justify-between items-center px-3 py-2">
            <div class="px-4 py-3">
                <a href="index.html" class="logo dark:hidden"><img src="@/assets/img/icon.png" alt="Logo Azkazikna"
                        class="w-[45px] lg:w-[55px]"></a>
                <a href="index.html" class="logo hidden dark:block"><img src="@/assets/img/icon.png" alt="Logo Azkazikna"
                        class="w-[85px]"></a>
            </div>
            <button class="hamburger px-4 py-3 lg:hidden" type="button">
                <span class="hamburger-line origin-top-left transition duration-300 ease-in-out"></span>
                <span class="hamburger-line transition duration-300 ease-in-out"></span>
                <span class="hamburger-line origin-bottom-left transition duration-300 ease-in-out"></span>
            </button>
            <nav class="hidden absolute top-full right-4 px-4 py-4 min-w-[250px] dark:border-white lg:static lg:block lg:border-0 bg-blackval dark:bg-background dark:border-opacity-20 dark:lg:bg-transparent lg:bg-transparent lg:shadow-none"
                data-barba-prevent="all">
                <ul class="lg:flex gap-5 items-center">
                    <li
                        class="text-lightval dark:text-white text-base dark:font-extralight mt-3 hover:scale-105 transition duration-300 ease-linear lg:mt-0">
                        <a id="nav-items" href="#about">About
                        </a>
                    </li>
                    <li
                        class="text-lightval dark:text-white text-base dark:font-extralight mt-3 hover:scale-105 transition duration-300 ease-linear lg:mt-0">
                        <a id="nav-items" href="#work">
                            Experience
                        </a>
                    </li>
                    <li
                        class="text-lightval dark:text-white text-base dark:font-extralight mt-3 hover:scale-105 transition duration-300 ease-linear lg:mt-0">
                        <a id="nav-items" href="#built">
                            Work
                        </a>
                    </li>
                    <li
                        class="text-lightval dark:text-white text-base dark:font-extralight mt-3 hover:scale-105 transition duration-300 ease-linear lg:mt-0">
                        <a id="nav-items" href="#contact">Contact
                        </a>
                    </li>
                    <li class="mt-3 lg:mt-0">
                        <a id="nav-items" href="dist/pdf/resume.pdf"
                            class="buttonAnimate relative text-lightval dark:text-primary dark:font-extralight border-[1px] py-2 px-2 border-lightval dark:border-primary hover:text-bgLight dark:hover:text-background hover:border-background transition duration-300 ease-in">
                            Resume
                        </a>
                    </li>
                    <li class="ml-4 mt-6 lg:mt-0">
                        <input type="checkbox" class="opacity-0 absolute top-0 group" id="toggleMode">
                        <label for="toggleMode"
                            class="w-[50px] h-[26px] bg-lightval flex rounded-full items-center justify-between p-[5px] relative scale-150 transition duration-300 ease-linear cursor-pointer">
                            <i class="fas fa-moon text-blackval"></i>
                            <i class="fa-solid fa-sun text-blackval text-sm"></i>
                            <div
                                class='ball w-5 h-5 bg-blackval absolute t-[2px] l-[2px] rounded-full transition duration-200 ease-linear'>
                            </div>
                        </label>
                    </li>
                </ul>
            </nav>
        </div>
    </header>

  <RouterView />

  <!-- footer start -->
  <footer id="footer">
        <div class="container px-4 py-8 mx-auto">
            <p class="dark:font-extralight text-base dark:text-secondary text-center">Built by <a
                    href="https://github.com/azkazikna" class="dark:text-white font-semibold">Azkazikna Ageung
                    Laksana</a> Inspired by <a href="https://playvalorant.com/id-id/"
                    class="dark:text-white font-semibold uppercase">Valorant</a></p>
        </div>
    </footer>
    <!-- footer end -->
</template>
