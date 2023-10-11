<script setup>
  import { Navbar, NavbarLogo, NavbarCollapse, NavbarLink } from 'flowbite-vue'
</script>

<template>
    <Navbar>
      <template #logo>
        <NavbarLogo link="/" alt="MEGA League" image-url="../assets/logo-dark.svg"> </NavbarLogo>
      </template>
      <template #default="{isShowMenu}">
        <NavbarCollapse :isShowMenu="isShowMenu">
          <NavbarLink is-active className="navLink">Home</NavbarLink>
          <NavbarLink className="navLink">Events</NavbarLink>
          <NavbarLink className="navLink">Impact</NavbarLink>
        </NavbarCollapse>
      </template>
      <template #right-side>
        <button type="button" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center mr-3 md:mr-0 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Sign in</button>
      </template>
    </Navbar>
</template>
<script>
export default {
    name: "NavigationBar"
}
</script>

<style scoped>
    .flex-container {
        display: flex;
        justify-content: space-between;
    }

    .links {
        margin: auto;
    }

    button {
      color: white;
      background: black;
      font-size: 1.5em;
      padding-top: 10px;
      padding-bottom: 10px;
      padding-left: 5px;
      padding-right: 5px;
    }

    .navLink {
      font-size: 1.5em;
    }

</style>