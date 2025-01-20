<script lang="ts">
  const { previousLevel, newLevel } = $props();
</script>

<div id="details">
  <header>
    <div id="icon">
      <img
        src="/public/friend.png"
        width="64px"
        height="64px"
        alt="Dog friend icon"
      />
    </div>
    <h1>Friendship Level Up!</h1>
  </header>
  <div id="level-change">
    <span class="level">{previousLevel}</span>
    <span>=></span>
    <span class="level">{newLevel}</span>
  </div>
  <div id="screen-title">
    <h2>Here's your Reward!</h2>
  </div>
</div>

<style>
  #details {
    position: sticky;
    top: 0px;
    background-color: #fec844;
    padding-bottom: 20px;
  }
  header {
    background-color: #ffdd86;
    flex-direction: row;
    min-height: 36px;
    position: relative;
    margin-top: 30px;
    align-items: center;
  }

  header #icon {
    position: absolute;
    top: -10px;
    left: 12px;

    width: 78px;
    height: 78px;
    border-radius: 50%;
    background-color: white;

    justify-content: center;
    align-items: center;
  }

  #icon img {
    transform: rotate(-15deg);
  }

  header h1 {
    flex: 1;
    text-align: center;
    margin-left: 96px;
    margin-right: 20px;
    padding: 4px 0;
    font-size: 20px;
    color: #f48412;
    font-family: "Humming";
  }

  #level-change {
    position: relative;
    top: -6px;
    flex-direction: row;
    justify-content: flex-end;
    align-items: center;
    gap: 4px;
    padding: 0 18px;
  }

  .level {
    background-color: #e84761;
    width: 30px;
    height: 30px;
    justify-content: center;
    align-items: center;
    color: white;
    font-family: "Humming";
    font-weight: 300;
  }

  #screen-title {
    text-align: center;
    color: #565458;
    font-family: Humming;
    background-color: #fbf6e3;
    margin: 0 30px;
    padding: 3px 0;
    border-radius: 30px;
    font-size: 12px;
  }
</style>
