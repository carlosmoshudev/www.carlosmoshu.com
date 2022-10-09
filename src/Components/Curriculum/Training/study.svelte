<script lang="ts">
  export let title: string;
  export let place: string;
  export let date: string;
  export let image: string;
</script>

<div class="study_card">
  <div class="relative_date_container"><p class="study_date">{date}</p></div>
  <div class="image_title">
    <img src={image} alt={place} />
    <h4 class="study_name">{title}</h4>
    <h5 class="study_place">{place}</h5>
  </div>
</div>

<style>
  .study_card {
    background-color: #fff;
    border-radius: 0.5rem;
    border: 1px solid #e1e4e8;
    padding: 1rem;
    margin-bottom: 1rem;
    transition: all 0.3s ease;
  }
  .study_card:hover {
    border: 1px solid #0366d6;
    box-shadow: 0 0 0 1px #0366d6, 0 4px 8px 0 rgba(3, 102, 214, 0.12);
  }
  .image_title {
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-radius: 1rem;
  }
  .study_card img {
    width: 4rem;
    height: 4rem;
    border-radius: 1rem 0 0 1rem;
    transition: all 0.3s ease;
    box-shadow: 0 0 0 1px #e1e4e8, 0 4px 8px 0 rgba(3, 102, 214, 0.12);
  }
  .study_card img:hover {
    transform: scale(1.1);
  }
  .study_name {
    font-size: 1.2rem;
    font-weight: 600;
    margin: 0;
    transition: all 0.3s ease;
  }
  .study_name:hover {
    color: #0366d6;
    transform: scale(1.1);
  }
  .study_place {
    font-size: 0.8rem;
    font-weight: 400;
    margin: 0;
  }
  /*
  * Date must be shown on the top right corner, decorated like a band
  */
  .relative_date_container {
    position: relative;
  }
  .study_date {
    position: absolute;
    top: -1rem;
    right: 0;
    font-size: 0.6rem;
    font-weight: 500;
    margin: 0;
    margin-left: 1rem;
    color: #586069;
    transform: rotate(30deg);
    background-color: #e1e4e8;
    padding: 0.5rem;
    border-radius: 0.5rem;
  }
</style>
