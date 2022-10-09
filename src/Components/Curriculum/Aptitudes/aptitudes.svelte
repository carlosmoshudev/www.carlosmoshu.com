<script lang="ts">
  import Languages from "./languages.svelte";
  import Skills from "./skills.svelte";
  import Technologies from "./technologies.svelte";
</script>

<h2>Aptitudes</h2>
<div class="aptitude_container"><Skills /></div>
<div class="aptitude_container"><Technologies /></div>
<div class="aptitude_container"><Languages /></div>

<style>
  .aptitude_container {
    background-color: #fff;
    border-radius: 0.5rem;
    border: 1px solid #e1e4e8;
    padding: 1rem;
    margin-bottom: 1rem;
    transition: all 0.3s ease;
    width: 90%;
  }
  .aptitude_container:hover {
    border: 1px solid #0366d6;
    box-shadow: 0 0 0 1px #0366d6, 0 4px 8px 0 rgba(3, 102, 214, 0.12);
  }
</style>
