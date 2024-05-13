<template>
  <nav>
    <ul>
      <li>
        <NuxtLink to="/">Home</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/about">About</NuxtLink>
      </li>
    </ul>
  </nav>
</template>

<style lang="postcss">
ul {
  @apply flex p-4;
  li {
    @apply p-4;
  }
}
</style>
