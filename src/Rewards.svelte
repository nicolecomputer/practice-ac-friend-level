<script>
  import Reward from "./Reward.svelte";
</script>

<div id="rewards">
  <Reward title="Bells" amount={200} />
  <Reward title="natural essence" amount="x1" />
  <Reward title="steel" amount="x3" />
  <Reward title="cotton" amount="x2" />
</div>

<style>
  #rewards {
    margin: 20px 12px;
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 12px;
    list-style: none;
    padding-left: 0;
  }
</style>
