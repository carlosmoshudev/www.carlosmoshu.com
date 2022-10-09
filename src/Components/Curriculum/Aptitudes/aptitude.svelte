<script lang="ts">
  export let title: string;
  export let progress: number;
  export let color: string;
</script>

<!--
  title and progress bar 
 -->
<div class="aptitude_card">
  <h4 class="aptitude_title">{title}</h4>
  <div class="progress_bar">
    <div
      class="progress"
      style={`width: ${progress}%; background-color: ${color};`}
    />
  </div>
</div>

<style>
  .aptitude_card {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 0.3rem;
    margin-bottom: 0.7rem;
  }

  .aptitude_title {
    font-size: 1rem;
    font-weight: 600;
    margin: 0;
  }
  .progress_bar {
    width: 100%;
    height: 0.4rem;
    border-radius: 0.5rem;
    background-color: #e1e4e8;
    margin-top: 0.5rem;
    transition: all 0.3s ease;
  }
  .progress {
    height: 100%;
    border-radius: 0.4rem;
    transition: all 0.3s ease;
  }
</style>
