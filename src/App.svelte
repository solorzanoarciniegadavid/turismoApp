<script>
  import logo from './assets/svelte.png'
  import Counter from './lib/Counter.svelte'
  import Navbar from './Navbar.svelte'
  import Banner from './Banner.svelte';
import TripCard from './TripCard.svelte';
import Footer from './Footer.svelte';
</script>

<link href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">

<Navbar />
<Banner />
<main>
  <TripCard />
</main>
<Footer />

<style>
  :root {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
      Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }

  main {
    text-align: center;
    padding: 1em;
    margin: 0 auto;
  }
</style>
