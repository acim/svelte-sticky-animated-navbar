<script>
  let y;
</script>

<style lang="scss">
  nav {
    position: fixed;
    text-align: right;
    float: right;
    width: 100%;
    transition: all 0.5s;
    padding: 10px;
    z-index: 1;
  }
  ul {
    list-style-type: none;

    li {
      display: inline-block;
      color: var(--color-heading);
    }
  }

  .pin {
    background: rgba(0, 0, 0, 0.6);
    color: white;
  }
</style>

<nav class:pin={y > 50}>
  <ul>
    <li>Portfolio</li>
    <li>About</li>
    <li>Contact</li>
  </ul>
</nav>

<svelte:window bind:scrollY={y} />
