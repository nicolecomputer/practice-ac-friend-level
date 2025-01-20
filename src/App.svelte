<script lang="ts">
  import LevelUpHeader from "./LevelUpHeader.svelte";
  import Rewards from "./Rewards.svelte";
</script>

<main>
  <LevelUpHeader previousLevel={1} newLevel={2} />
  <div id="rewards">
    <Rewards />
  </div>
  <div id="button-area">
    <button>OK</button>
  </div>
</main>

<style>
  #rewards {
    min-height: 80vh;
  }
  #button-area {
    position: sticky;
    bottom: 0;
    background-color: #fec844;
    padding: 10px;
    align-content: center;
    justify-content: center;
    width: 100%;
  }

  button {
    height: 48px;
    text-align: center;
    width: min-content;
    padding: 20px 80px;
    justify-content: center;
    background-color: #075663;
    border: none;
    border-radius: 18px;
    color: white;
    font-family: Humming;
    box-shadow: 0 6px 0px #073a3d;
    align-self: center;
  }

  button:active {
    background-color: #073a3d;
    position: relative;
    top: 6px;
    box-shadow: none;
  }
</style>
