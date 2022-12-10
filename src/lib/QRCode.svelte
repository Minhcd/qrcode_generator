<script lang="ts">
  import QrCode from 'svelte-qrcode';

  let context: string = '';
</script>

<div class="qr">
  <QrCode value={context} size="300" />
  <input bind:value={context} placeholder="Enter your context" />
</div>

<style>
  .qr {
    width: 100%;
  }

  input {
    margin-top: 10px;
    width: 100%;
    border-radius: 5px;
    color: var(--dark-blue);
  }
</style>
