<script>
  export let title = "Art Website";
</script>

<style>
  header {
    background-color: #f8f9fa;
    padding: 1rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  h1 {
    margin: 0;
    font-size: 2rem;
    color: #333;
  }

  nav {
    display: flex;
    gap: 1rem;
  }

  a {
    text-decoration: none;
    color: #007bff;
  }

  a:hover {
    text-decoration: underline;
  }
</style>

<header>
  <h1>{title}</h1>
  <nav>
    <a href="/">Home</a>
    <a href="/about">About</a>
    <a href="/gallery">Gallery</a>
    <a href="/contact">Contact</a>
  </nav>
</header>