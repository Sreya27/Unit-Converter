<script>
  import Navbar from "../components/navbar.svelte";
  import Table from "../components/table.svelte";
</script>

<Navbar />
<Table />

<slot />

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;800&display=swap');

  :global(*){
      font-family: 'Inter', sans-serif;
      margin:0;
      padding: 0;
      box-sizing: border-box;
      text-decoration: none;
      color: var(--dark);
  }

  /* //color variables */

  :global(:root){
      --primary: #e03616;
      --secondary: #0066FF;
      --dark: #222;
      --light: #ebebeb;

  }

  :global(body){
      background-color: white;
  }

</style>