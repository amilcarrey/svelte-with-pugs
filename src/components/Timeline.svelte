<script>
  import Card from "./Card";
  export let posts = [];
</script>

<style>
  .TimeLine {
    padding: 4em 0 0 0;
  }
</style>

<div class="TimeLine">
  <div class="Timeline-container">
    {#each posts as post}
      <Card {...post}/>
    {:else}
      <p>Loading...</p>
    {/each}

  </div>
</div>
