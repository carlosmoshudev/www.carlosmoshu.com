<script lang="ts">
  export let title: string;
  export let color: string;
</script>

<!--
  title and progress bar 
 -->
<div class="aptitude_card" style="background-color: {color}">
  <h4 class="aptitude_title">{title}</h4>
</div>

<style>
  .aptitude_card {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 0;
    margin-bottom: 0.2rem;
    margin-right: 0.5rem;
    padding: 0.2rem 0.5rem;
    border-radius: 0.5rem;
    color: #fff;
  }

  .aptitude_title {
    font-size: 0.8rem;
    font-weight: 600;
    margin: 0;
  }
</style>
