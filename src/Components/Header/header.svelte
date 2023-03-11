<script lang="ts">
  import Header from "./header.svelte";
  import Curriculum from "./../../Pages/curriculum.svelte";
</script>

<header class="header">
  <div class="header_container">
    <div class="left_corner">
      <div class="github_card">
        <div class="github_card_container">
          <img
            src="https://github-readme-stats.vercel.app/api/top-langs/?username=carlosmoshudev&layout=compact&theme=default&count_private=true&hide_border=true&custom_title=Leguajes+más+usados+en+GitHub&langs_count=10"
            alt="GitHub Top Languages"
          />
        </div>
      </div>
    </div>
    <div class="main_header">
      <h1 class="title"><a href="/">Carlos Soto Pedreira</a></h1>
      <h2 class="subtitle">
        Sistemas · Telecomunicaciones · Desarrollo · Ciberseguridad
      </h2>
      <div class="header_nav">
        <nav>
          <ul class="header_nav_list">
            <li class="header_nav_item curriculum">
              <a href="/">Curriculum Vitae</a>
            </li>
            <li class="header_nav_item social">
              <a href="/socialnetworks">Redes Sociales</a>
            </li>
            <li class="header_nav_item matrix">
              <a href="/skillmatrix">Matriz de Habilidades</a>
            </li>
            <li class="header_nav_item projects">
              <a href="/projects">Proyectos</a>
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </div>
</header>

<style>
  /* MUST USE THIS ICONS ON NAV

  curriculum url("https://cdn-icons-png.flaticon.com/512/3135/3135686.png");
  social url("https://cdn-icons-png.flaticon.com/512/2065/2065064.png");
  matrix url("https://cdn-icons-png.flaticon.com/512/2065/2065092.png");
  projects url("https://cdn-icons-png.flaticon.com/512/2065/2065118.png");
  */
  /* Header is sticky and white */
  .header {
    position: sticky;
    top: 0;
    z-index: 100;
    background-color: white;
    box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.1);
    margin-right: 0;
  }
  .header_container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    padding: 0 1rem;
    max-width: 1200px;
    margin: 0;
    margin-right: 0;
  }
  .left_corner {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: center;
  }
  .github_card {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: center;
    margin-left: 1rem;
  }
  .github_card_container {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: center;
    width: 300px;
    height: 100px;
  }
  .main_header {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-right: 0;
    margin-left: 2rem;
    margin-bottom: 2rem;
  }
  .title {
    font-size: 2rem;
    font-weight: 700;
    margin: 0;
    margin-bottom: 0.5rem;
    font-family: "Roboto", sans-serif;
  }
  .title a {
    color: #1e90ff;
    text-decoration: none;
  }
  .title a:hover {
    color: #1e90ff;
    text-decoration: underline;
  }
  .subtitle {
    font-size: 1rem;
    font-weight: 400;
    margin: 0;
    font-family: "Roboto", sans-serif;
    letter-spacing: 0.15rem;
  }
  .header_nav {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    margin-top: 1rem;
  }
  .header_nav_list {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    list-style: none;
    margin: 0;
    padding: 0;
  }
  .header_nav_item {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    margin: 0 0.5rem;
  }
  .header_nav_item a {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    text-decoration: none;
    color: #1e90ff;
    font-size: 1rem;
    font-weight: 400;
    font-family: "Roboto", sans-serif;
    letter-spacing: 0.02rem;
    margin-bottom: 3vh;
  }
  /* On hover has animated underline, transformed and animated */
  .header_nav_item a:hover {
    color: #1e90ff;
    text-decoration: underline;
    text-decoration-color: #1e90ff;
    text-decoration-thickness: 2px;
    text-underline-offset: 0.2rem;
    transform: translateX(0.2rem);
    transition: all 0.2s ease-in-out;
  }
  /* Curriculum icon */
  .header_nav_item.curriculum a::before {
    content: "";
    display: inline-block;
    width: 1.5rem;
    height: 1.5rem;
    margin-right: 0.5rem;
    background-image: url("https://cdn-icons-png.flaticon.com/512/3135/3135686.png");
    background-size: cover;
  }
  /* Social icon */
  .header_nav_item.social a::before {
    content: "";
    display: inline-block;
    width: 1.5rem;
    height: 1.5rem;
    margin-right: 0.5rem;
    background-image: url("https://cdn-icons-png.flaticon.com/512/2065/2065064.png");
    background-size: cover;
  }
  /* Matrix icon */
  .header_nav_item.matrix a::before {
    content: "";
    display: inline-block;
    width: 1.5rem;
    height: 1.5rem;
    margin-right: 0.5rem;
    background-image: url("https://cdn-icons-png.flaticon.com/512/2065/2065092.png");
    background-size: cover;
  }
  /* Projects icon */
  .header_nav_item.projects a::before {
    content: "";
    display: inline-block;
    width: 1.5rem;
    height: 1.5rem;
    margin-right: 0.5rem;
    background-image: url("https://cdn-icons-png.flaticon.com/512/2065/2065118.png");
    background-size: cover;
  }
</style>
