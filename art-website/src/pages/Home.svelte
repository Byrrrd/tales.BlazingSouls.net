<script>
  import Header from '../components/Header.svelte';

  let featuredArtworks = [
    {
      title: 'Starry Night',
      artist: 'Vincent van Gogh',
      description: 'A depiction of a night sky filled with swirling clouds and stars.',
      imageUrl: 'path/to/starry-night.jpg'
    },
    {
      title: 'Mona Lisa',
      artist: 'Leonardo da Vinci',
      description: 'A portrait of a woman with a mysterious smile.',
      imageUrl: 'path/to/mona-lisa.jpg'
    },
    {
      title: 'The Persistence of Memory',
      artist: 'Salvador Dalí',
      description: 'A surrealistic painting featuring melting clocks.',
      imageUrl: 'path/to/persistence-of-memory.jpg'
    }
  ];
</script>

<Header />

<main>
  <h1>Welcome to the Art Gallery</h1>
  <section>
    <h2>Featured Artworks</h2>
    <div class="artwork-list">
      {#each featuredArtworks as artwork}
        <div class="artwork-item">
          <img src={artwork.imageUrl} alt={artwork.title} />
          <h3>{artwork.title}</h3>
          <p><strong>Artist:</strong> {artwork.artist}</p>
          <p>{artwork.description}</p>
        </div>
      {/each}
    </div>
  </section>
</main>

<style>
  main {
    padding: 20px;
    text-align: center;
  }

  .artwork-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }

  .artwork-item {
    margin: 15px;
    border: 1px solid #ccc;
    border-radius: 8px;
    padding: 10px;
    width: 200px;
  }

  .artwork-item img {
    max-width: 100%;
    border-radius: 4px;
  }
</style>