<script lang="ts">
  import Job from "./job.svelte";
</script>

<article>
  <h2>Experiencia Profesional</h2>
  <Job
    enterprise="Inelcom S.A."
    years={{ start: 2020 }}
    description={["Técnico de Sistemas Nivel 2 - Inditex"]}
    img="../../../img/inelcom.png"
    tasks={[
      "Soporte y provisión de aplicaciones de punto de venta.",
      "Administración y diagnóstico de sistemas Windows y periféricos",
      "Instalación y mantenimiento de base de datos MSSQL",
      "Gestión de incidencias y activos en Remedy y Jira",
      "Gestión de equipos en Active Directory",
      "Soporte e instalación RFID, Pinpads, Impresoras, Escáneres y Displays",
    ]}
    skills={[
      "Scripting en Powershell - Automatización de diagnósticos y procesos",
      "Desarrollo de microutiles en C# .NET - Automatización de reportes y tipificaciones",
    ]}
    technologies={[
      "Windows Server 2012 R2",
      "Windows 10",
      "MSSQL",
      "Active Directory",
      "Remedy",
      "Jira",
      "Powershell",
      "C# .NET",
      "Power Query",
      "Grafana",
    ]}
  />
  <Job
    enterprise="Oesía Networks S.L."
    years={{ start: 2019, end: 2021 }}
    description={[
      "Operador de Redes CG CORA - SGAD",
      "Técnico de Redes - Inditex",
    ]}
    img="../../../img/oesia.png"
    tasks={[
      "Recepción, diagnóstico y gestión o asignación de incidencias.",
      "Deteción proactiva de incomunicaciones con dashboards de monitorización.",
      "Creación de incidencias proactivas en EasyVista y Vantive.",
      "Creación de informes rutinarios de alertas de red.",
      "Soporte a infraestructura de redes y voIP.",
    ]}
    skills={[
      "Desarrollo en Excel, PowerQuery y Macros VB - Automatización de informes.",
      "Gestión de Base de Conocimiento en TikiWiki.",
    ]}
    technologies={[
      "Vantive",
      "EasyVista",
      "WOCU",
      "Macros VisualBasic",
      "Unify",
      "Cisco",
    ]}
    tasks2={[
      "Analítica de topología de red de cliente.",
      "Gestión de implantaciones de red.",
      "Gestión de rangos IP con IPAM.",
      "Configuración de Controladoras Aruba para routing.",
      "Configuración de Switches Aruba.",
      "Configuración de APs modo Campus.",
      "Asistencia y soporte a despliegues y post despliegues.",
      "Resolución de incidencias de red, confiuración DHCP, Radius, Cableado",
      "Configuración de Paths en Firewalls Palo Alto.",
    ]}
    skills2={[
      "Scripting en Python - Automatización de consolas SecureCRT.",
      "Gestión de Base de Conocimiento en Confluence.",
      "Desarrollo de microutilidad en C# .NET - Consulta masiva de MAC por API para Radius.",
    ]}
    technologies2={[
      "Aruba",
      "Palo Alto",
      "Python",
      "C# .NET",
      "SecureCRT",
      "Confluence",
      "Remedy",
      "IPAM",
      "ClearPass",
    ]}
  />
  <Job
    enterprise="Teleperformance España S.A."
    years={{ start: 2018, end: 2019 }}
    description={["Teleoperador Atención al Cliente - Orange"]}
    img="../../../img/teleperformance.png"
    tasks={[
      "Atención telefónica a clientes de Orange.",
      "Soporte técnico FTTH, ADSL, IPTV, Móvil, Fijo, VoIP.",
      "Diagnóstico de Incidencias.",
      "Gestión de Facturación.",
      "Gestión de proceso de Provisión de servicios.",
    ]}
    skills={["Formación técnica y metodología de atención al cliente."]}
    technologies={[
      "Siebel 7",
      "Siebel 8",
      "Ficha de Cliente",
      "Altitude",
      "Altair",
      "Avaya VoIP",
      "ICP",
      "BSCS",
    ]}
  />
  <Job
    enterprise="Hispatel Soluciones S.L."
    years={{ start: 2017, end: 2018 }}
    description={["Técnico de sistemas, redes y gestión administrativa"]}
    img="../../../img/hispatel.png"
    tasks={[
      "Gestión de proyectos de Cartelería Digital con BrightSign.",
      "Gestión de proyectos de CCTV y Cámaras IP.",
      "Gestión de centralitas y dispositivos VoIP, digitales y analógicos.",
      "Gestión de VPNs y redes de voz y datos.",
      "Configuración de electrónica de red, Routers, Modems, Switches.",
      "Tratamiento y gestión documental.",
      "Atención al cliente y asesoramiento técnico.",
    ]}
    skills={[
      "Automatización de sistemas Android con Tasker.",
      "Creación de contenidos de formación y gestión de bases de conocimiento Goldmine.",
    ]}
    technologies={[
      "BrightSign",
      "Goldmine",
      "Tasker",
      "Android",
      "Draytek",
      "Panasonic",
    ]}
  />
  <Job
    enterprise="Bricoking S.L."
    years={{ start: 2013, end: 2013 }}
    description={["Área de ventas · FCT Gestión Administrativa"]}
    img="../../../img/bricoking.png"
    tasks={[
      "Gestión de almacén y puenting de pedidos.",
      "Atención al cliente y asesoramiento técnico.",
      "Reposición de mercancía.",
      "Mezcla de pinturas.",
    ]}
    skills={[]}
    technologies={[]}
  />
  <Job
    enterprise="Sykes Enterprises S.L."
    years={{ start: 2011, end: 2011 }}
    description={["IT Helpdesk · FCT Sistemas y Redes"]}
    img="../../../img/sykes.png"
    tasks={[
      "Gestión de incidencias de equipos informáticos y periféricos.",
      "Gestión de incidencias de redes de cableado y configuración de routers.",
      "Administración de usuarios y grupos de dominio.",
      "Gestión de cortafuegos.",
      "Administración de redes LAN.",
      "Gestión de contenidos SharePoint.",
    ]}
    skills={[]}
    technologies={[
      "SharePoint",
      "Active Directory",
      "Windows Server",
      "Windows 7",
      "Outlook",
    ]}
  />
</article>

<style>
</style>
