<script lang="ts">
  export let enterprise: string;
  export let years: { start: number; end?: number };
  export let description: Array<string>;
  export let img: string;
  export let tasks: Array<string>;
  export let skills: Array<string>;
  export let technologies: Array<string>;
  export let tasks2: Array<string> = [];
  export let skills2: Array<string> = [];
  export let technologies2: Array<string> = [];
</script>

<div class="company">
  <div class="company_header">
    <img class="logo" src={img} alt={enterprise} />
    <h3 class="company_name">{enterprise}</h3>
    {#if years.end && years.end !== years.start}
      <p class="years">
        {years.start} - {years.end}
        <span class="time"> {years.end - years.start} Año(s)</span>
      </p>
    {:else if years.end && years.end === years.start}
      <p class="years">
        {years.start}
        <span class="time"> &#60; 1 Año</span>
      </p>
    {:else}
      <p class="years">
        {years.start} - Actualidad
        <span class="time">
          {new Date().getFullYear() - years.start} Año(s)
        </span>
      </p>
    {/if}
  </div>
  <div class="position">
    <h4 class="description">{description[0]}</h4>
    <div class="lists">
      <p>Funciones principales:</p>
      <ul class="task_list">
        {#each tasks as task}
          <li class="task">{task}</li>
        {/each}
      </ul>
      <div class="position_skills">
        <p>Habilidades desarrolladas:</p>
        <ul class="skill_list">
          {#each skills as skill}
            <li class="skill">{skill}</li>
          {/each}
        </ul>
      </div>
      <div class="technologies">
        <p>Tecnologías utilizadas:</p>
        <ul class="technology_list">
          {#each technologies as technology}
            <li class="technology">{technology}</li>
          {/each}
        </ul>
      </div>
    </div>
    {#if description.length > 1}
      <div class="position">
        <h4 class="description">{description[1]}</h4>
        <div class="lists">
          <p>Funciones principales:</p>
          <ul class="task_list">
            {#each tasks2 as task}
              <li class="task">{task}</li>
            {/each}
          </ul>
          <div class="position_skills">
            <p>Habilidades desarrolladas:</p>
            <ul class="skill_list">
              {#each skills2 as skill}
                <li class="skill">{skill}</li>
              {/each}
            </ul>
          </div>
          <div class="technologies">
            <p>Tecnologías utilizadas:</p>
            <ul class="technology_list">
              {#each technologies2 as technology}
                <li class="technology">{technology}</li>
              {/each}
            </ul>
          </div>
        </div>
      </div>
    {/if}
  </div>
</div>

<style>
  .company {
    background-color: #fff;
    border-radius: 0.5rem;
    border: 1px solid #e1e4e8;
    padding: 1rem;
    margin-bottom: 1rem;
    transition: all 0.3s ease;
  }
  .company:hover {
    border: 1px solid #0366d6;
    box-shadow: 0 0 0 1px #0366d6, 0 4px 8px 0 rgba(3, 102, 214, 0.12);
  }
  .company_header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-radius: 1rem;
  }
  .logo {
    width: 4rem;
    height: 4rem;
    border-radius: 1rem 0 0 1rem;
    transition: all 0.3s ease;
    box-shadow: 0 0 0 1px #e1e4e8, 0 4px 8px 0 rgba(3, 102, 214, 0.12);
  }
  .logo:hover {
    transform: scale(1.1);
  }
  .company_name {
    font-size: 1.2rem;
    font-weight: 600;
    margin: 0;
    transition: all 0.3s ease;
  }
  .company_name:hover {
    color: #0366d6;
    transform: scale(1.1);
  }
  .years {
    font-size: 0.8rem;
    font-weight: 400;
    margin: 0;
  }
  .time {
    font-size: 0.6rem;
    font-weight: 500;
    margin: 0;
    margin-left: 1rem;
    color: #586069;
  }
  .position {
    text-align: left;
  }
  .description {
    font-size: 1.2rem;
    font-weight: 600;
    margin: 0;
    margin-top: 1rem;
    color: #f9826c;
  }
  .lists {
    border-top: 1px solid #f9826c;
    border-left: 1px solid #f9826c;
    padding-left: 1rem;
  }
  /* parragraphs styled
  * list items has indentations bleeding
  */
  .lists p {
    margin: 0;
    margin-top: 1rem;
    font-size: 1rem;
    font-weight: 600;
    color: #586069;
  }
  .task_list {
    list-style: none;
    padding: 0;
    padding-left: 1.5rem;
    margin: 0;
    margin-top: 0.5rem;
  }
  .task {
    font-size: 0.8rem;
    font-weight: 400;
    margin: 0;
    margin-bottom: 0.2rem;
  }
  .task::before {
    content: "•";
    color: #f9826c;
    display: inline-block;
    width: 1rem;
    margin-left: -1rem;
  }
  .position_skills {
    margin-top: 1rem;
  }
  .skill_list {
    list-style: none;
    padding: 0;
    padding-left: 1.5rem;
    margin: 0;
    margin-top: 0.5rem;
  }
  .skill {
    font-size: 0.8rem;
    font-weight: 400;
    margin: 0;
    margin-bottom: 0.2rem;
  }
  .skill::before {
    content: "•";
    color: #f9826c;
    display: inline-block;
    width: 1rem;
    margin-left: -1rem;
  }
  /*
  * Technologies list items displayed inline with button style, there are tags
  */
  .technologies {
    margin-top: 1rem;
  }
  .technology_list {
    list-style: none;
    padding: 0;
    padding-left: 1.5rem;
    margin: 0;
    margin-top: 0.5rem;
    display: flex;
    flex-wrap: wrap;
  }
  .technology {
    font-size: 0.8rem;
    font-weight: 400;
    margin: 0;
    margin-bottom: 0.2rem;
    margin-right: 0.5rem;
    padding: 0.2rem 0.5rem;
    border-radius: 0.5rem;
    background-color: #f9826c;
    color: #fff;
  }
  .technology:hover {
    background-color: #f25c2c;
    cursor: pointer;
  }
</style>
