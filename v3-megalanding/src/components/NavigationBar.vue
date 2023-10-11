<script setup>
import { Navbar, NavbarLogo, NavbarCollapse, NavbarLink } from 'flowbite-vue'
import { Button } from 'flowbite-vue'
</script>
<template>
    <Navbar>
      <template #logo>
        <NavbarLogo link="/" alt="Flowbite logo" image-url="../assets/logo-dark.svg">
        </NavbarLogo>
      </template>
      <template #default="{isShowMenu}">
        <NavbarCollapse :isShowMenu="isShowMenu">
          <NavbarLink isActive link="#">Home</NavbarLink>
          <NavbarLink link="#">Events</NavbarLink>
          <NavbarLink link="#">Impact</NavbarLink>
          <Button color="dark">Sign in</Button>
        </NavbarCollapse>
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

</style>