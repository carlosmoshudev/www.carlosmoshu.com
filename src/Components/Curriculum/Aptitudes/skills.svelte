<script lang="ts">
  import Aptitude from "./aptitude.svelte";
</script>

<h3 class="title">Habilidades</h3>
<div class="skill_container">
  <Aptitude title="Desarrollo de Software" progress={90} color="#0366d6" />
  <Aptitude title="Administración de sistemas" progress={80} color="#0366d6" />
  <Aptitude title="Administración de redes" progress={100} color="#0366d6" />
  <Aptitude title="Ofimática avanzada" progress={85} color="#0366d6" />
  <Aptitude title="SEO y SEM" progress={70} color="#0366d6" />
  <Aptitude title="Diseño de experiencia UX" progress={65} color="#0366d6" />
  <Aptitude title="Gestión de proyectos" progress={60} color="#0366d6" />
  <Aptitude title="Formación y documentación" progress={80} color="#0366d6" />
</div>

<style>
  .skill_container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    grid-gap: 1rem;
    border-top: 1px solid #0366d6;
    padding-top: 1rem;
    border-left: 1px solid #0366d6;
    padding-left: 1rem;
  }
</style>
