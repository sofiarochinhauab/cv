<template>
  <header>
    <img alt="Vue logo" src="../assets/avatar.png" height="50" />
    <p>Meu currículo</p>
    <nav>
      <ul>
        <li><router-link to="/">Quem sou eu?</router-link></li>
        <li><router-link to="/about">O que faço?</router-link></li>
        <li><router-link to="/hobbies">Hobbies</router-link></li>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss">
header {
  display: flex;
  border-bottom: 1px solid #ccc;
  padding: 0.5rem 1rem;

  p {
    margin-left: 1rem;
  }
}

nav {
  margin-left: auto;

  ul {
    list-style: none;
  }

  ul li {
    display: inline-flex;
    margin-left: 1rem;
  }
}
</style>
<script setup></script>
