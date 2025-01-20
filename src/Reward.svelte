<script lang="ts">
  const { title, amount } = $props();
</script>

<div class="reward">
  <div class="icon"></div>
  <h4>{title}</h4>
  <p class="amount">{amount}</p>
  <p class="already-have"><span class="have-icon"></span> 2</p>
</div>

<style>
  .reward {
    min-height: 140px;

    align-items: center;
  }

  .icon {
    width: 60px;
    height: 60px;
    background-color: #faf5e2;
    border-radius: 50%;
  }

  h4 {
    font-family: Humming;
    text-align: center;
    font-size: 12px;
  }

  .amount {
    font-family: Humming;
    font-size: 12px;
    background-color: #ebe4ca;
    min-width: 60px;
    border-radius: 9px;
    text-align: center;
  }

  .already-have {
    margin-top: 4px;
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 3px;
    font: Humming;
    color: #f37e0b;
  }
  .have-icon {
    width: 10px;
    height: 10px;
    border-radius: 2px;
    background-color: #f37e0b;
  }
</style>
