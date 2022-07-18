<script>
  import logo from './assets/svelte.png'
  import Counter from './lib/Counter.svelte'
  import Navbar from './Navbar.svelte'
  import Banner from './Banner.svelte';
import TripCard from './TripCard.svelte';
import Footer from './Footer.svelte';
import Person from './Person.svelte';
import Skills from './Skills.svelte';
import Input from './Input.svelte';

const data = {
  name: "David",
  lastname: "Solorzano",
  age: 27
}

let styles = {
  darkMode : false
}

function toggle(){
  styles.darkMode = !styles.darkMode;
  window.document.body.classList.toggle("dark-mode");
}
</script>

<link href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">

<Navbar />
<Banner />
<main>
  <TripCard />
</main>
<Footer />

<Person {...data} />
<button on:click={toggle}>Dark</button>

<Skills />
<Input />

{#if !styles.darkMode}
  <p>Holi</p>
{:else}
  <p>Holi else</p>
{/if}
<style>
  :root {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
      Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }

  :global(body.dark-mode){
    background-color: #1d3041;
    color: white;
  }

  main {
    text-align: center;
    padding: 1em;
    margin: 0 auto;
  }
</style>
