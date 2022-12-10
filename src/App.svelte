<script lang="ts">
  import favicon from './assets/favicon-32x32.png';
  import QRCode from './lib/QRCode.svelte';
</script>

<svelte:head>
  <link rel="icon" type="image/png" href={favicon} />
</svelte:head>
<main>
  <div class="container">
    <QRCode />
  </div>
</main>

<style>
  .container {
    max-width: 300px;
    min-height: 300px;
    margin: 0 auto;
    background-color: var(--white);
    padding: 15px;
    border-radius: 15px;
  }
</style>
