<script lang="ts">
  import Aptitude from "./aptitude.svelte";
</script>

<h3 class="title">Tecnologías</h3>
<h4 class="group">Desarrollo</h4>
<div class="desarrollo">
  <Aptitude title="PowerShell" progress={90} color="#9b4dca" />
  <Aptitude title="Visual Basic" progress={85} color="#9b4dca" />
  <Aptitude title="C# - .NET" progress={100} color="#9b4dca" />
  <Aptitude title="JavaScript" progress={65} color="#9b4dca" />
  <Aptitude title="TypeScript" progress={65} color="#9b4dca" />
  <Aptitude title="Svelte" progress={60} color="#9b4dca" />
</div>
<h4 class="group">Redes</h4>
<div class="redes">
  <Aptitude title="Draytek" progress={75} color="#9b4dca" />
  <Aptitude title="Cisco" progress={70} color="#9b4dca" />
  <Aptitude title="Palo Alto" progress={50} color="#9b4dca" />
  <Aptitude title="VMware" progress={80} color="#9b4dca" />
  <Aptitude title="Aruba" progress={100} color="#9b4dca" />
</div>
<h4 class="group">VoIP</h4>
<div class="voip">
  <Aptitude title="Cisco Call Manager" progress={60} color="#9b4dca" />
  <Aptitude title="Alcatel OXE" progress={50} color="#9b4dca" />
  <Aptitude title="Avaya" progress={60} color="#9b4dca" />
  <Aptitude title="Unify" progress={70} color="#9b4dca" />
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
