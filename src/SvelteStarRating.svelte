<script>
  let rating = 0;

  function setRating(value) {
    rating = value;
  }
</script>

<style>
  .star {
    display: inline-block;
    color: gold;
    cursor: pointer;
  }
</style>
  <!-- svelte-ignore a11y-click-events-have-key-events -->
<div>
  <span class="star" on:click={() => setRating(1)}>★</span>
  <span class="star" on:click={() => setRating(2)}>★</span>
  <span class="star" on:click={() => setRating(3)}>★</span>
  <span class="star" on:click={() => setRating(4)}>★</span>
  <span class="star" on:click={() => setRating(5)}>★</span>
</div>

<p>Rating: {rating} stars</p>

