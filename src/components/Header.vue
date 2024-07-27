<template>
  <header>
    <nav>
      <h1>
        <router-link to="/">Watching Party! 🥳</router-link>
      </h1>
      <ul>
        <li>
          <router-link to="/about">About</router-link>
        </li>
        <li>
          <router-link to="/room-list">Join room</router-link>
        </li>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 7svh;
  background-color: rgba($color: #000000, $alpha: 0.3);
  backdrop-filter: blur(8px) brightness(1.2);
  display: flex;
  justify-content: center;
  align-items: center;

  a {
    text-decoration: none;
    color: var(--gray-rgb);
    display: inline-block;
    padding: 0.75rem 1.5rem;
    border: 1px solid transparent;
    transition: color 0.15s;
  }

  a:active,
  a:hover,
  a.router-link-active {
    color: var(--bright);
    border: 1px solid var(--bright);
  }

  h1 a {
    color: var(--very-bright);
  }

  h1 a:hover,
  h1 a:active,
  h1 a.router-link-active {
    border-color: transparent;
  }

  nav {
    width: 90%;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  ul {
    list-style: none;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  li {
    margin: 0 0.5rem;
  }
}
</style>
