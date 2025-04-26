<script>
  import Footer from "./Footer.svelte";
  import Header from "./Header.svelte";
</script>

<Header />
<main class="container">
  <video src="/video/street.mp4" autoplay loop muted></video>
</main>
<Footer />

<style>
  video {
    width: 100%;
    aspect-ratio: 2.35/1;
    object-fit: cover;
    object-position: center;
  }
</style>
