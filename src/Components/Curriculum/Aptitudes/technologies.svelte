<script lang="ts">
  import Aptitude from "./aptitude.svelte";
</script>

<h3 class="title">Tecnologías</h3>
<h4 class="group">Desarrollo</h4>
<div class="desarrollo">
  <Aptitude title="PowerShell" color="#9b4dca" />
  <Aptitude title="Visual Basic" color="#9b4dca" />
  <Aptitude title="C# - .NET" color="#9b4dca" />
  <Aptitude title="JavaScript" color="#9b4dca" />
  <Aptitude title="TypeScript" color="#9b4dca" />
  <Aptitude title="Svelte" color="#9b4dca" />
</div>
<h4 class="group">Redes</h4>
<div class="redes">
  <Aptitude title="Draytek" color="#9b4dca" />
  <Aptitude title="Cisco" color="#9b4dca" />
  <Aptitude title="Palo Alto" color="#9b4dca" />
  <Aptitude title="VMware" color="#9b4dca" />
  <Aptitude title="Aruba" color="#9b4dca" />
</div>
<h4 class="group">VoIP</h4>
<div class="voip">
  <Aptitude title="Cisco Call Manager" color="#9b4dca" />
  <Aptitude title="Alcatel OXE" color="#9b4dca" />
  <Aptitude title="Avaya" color="#9b4dca" />
  <Aptitude title="Unify" color="#9b4dca" />
</div>

<style>
  .group {
    margin-top: 1rem;
  }
  .desarrollo {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    grid-gap: 1rem;
    border-top: 1px solid #9b4dca;
    padding-top: 1rem;
    border-left: 1px solid #9b4dca;
    padding-left: 1rem;
  }
  .redes {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    grid-gap: 1rem;
    border-top: 1px solid #9b4dca;
    padding-top: 1rem;
    border-left: 1px solid #9b4dca;
    padding-left: 1rem;
  }
  .voip {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    grid-gap: 1rem;
    border-top: 1px solid #9b4dca;
    padding-top: 1rem;
    border-left: 1px solid #9b4dca;
    padding-left: 1rem;
  }
</style>
