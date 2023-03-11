<script lang="ts">
  import Aptitude from "./aptitude.svelte";
</script>

<h3 class="title">Idiomas</h3>
<div class="language_container">
  <Aptitude title="Español" color="#cbbd52" />
  <Aptitude title="Gallego" color="#cbbd52" />
  <Aptitude title="Inglés" color="#cbbd52" />
  <Aptitude title="Portugués" color="#cbbd52" />
  <Aptitude title="Chino Mandarín" color="#cbbd52" />
</div>

<style>
  .language_container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    grid-gap: 1rem;
    border-top: 1px solid #cbbd52;
    padding-top: 1rem;
    border-left: 1px solid #cbbd52;
    padding-left: 1rem;
  }
</style>
