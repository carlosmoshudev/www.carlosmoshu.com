<script lang="ts">
  import Aptitude from "./aptitude.svelte";
</script>

<h3 class="title">Idiomas</h3>
<div class="language_container">
  <Aptitude title="Español" progress={100} color="#f1e05a" />
  <Aptitude title="Gallego" progress={100} color="#f1e05a" />
  <Aptitude title="Inglés" progress={70} color="#f1e05a" />
  <Aptitude title="Portugués" progress={80} color="#f1e05a" />
  <Aptitude title="Chino Mandarín" progress={55} color="#f1e05a" />
</div>

<style>
  .language_container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    grid-gap: 1rem;
    border-top: 1px solid #f1e05a;
    padding-top: 1rem;
    border-left: 1px solid #f1e05a;
    padding-left: 1rem;
  }
</style>
