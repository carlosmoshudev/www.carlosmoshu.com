<script lang="ts">
  import Aptitudes from "../Components/Curriculum/Aptitudes/aptitudes.svelte";
  import Experience from "../Components/Curriculum/Experience/experience.svelte";
  import Training from "../Components/Curriculum/Training/training.svelte";
</script>

<div id="home_container">
  <div class="left_column">
    <Experience />
  </div>
  <div class="right_column">
    <Training />
    <Aptitudes />
  </div>
</div>

<style>
  #home_container {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    background-color: #f5f5f5;
    color: #000000;
  }
  .left_column {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 50%;
    padding: 1rem;
  }
  .right_column {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 50%;
    padding: 1rem;
  }
  @media only screen and (max-width: 600px) {
    #home_container {
      flex-direction: column;
    }
    .left_column {
      width: 100%;
    }
    .right_column {
      width: 100%;
    }
  }
</style>
