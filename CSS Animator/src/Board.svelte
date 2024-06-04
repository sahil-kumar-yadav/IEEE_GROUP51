<script>
  import Boardbody from "./Boardbody.svelte";

  import Boardhead from "./Boardhead.svelte";

  import Action from "./Action.svelte";

  import Actionbar from "./Actionbar.svelte";
</script>

<div class="board">
  <Boardhead />
  <Boardbody />
</div>

<style>
  .board {
    width: 100%;
    height: 100%;
    max-height: 100%;
    background-color: rgba(173, 216, 230, 0.822);
    /* background: linear-gradient(90deg, #f6f5fa 28px, transparent 1%) 50%,
      linear-gradient(#f6f5fa 28px, transparent 1%) 50%, #d2cde6; */
    background-size: auto, auto, auto;
    background-size: 30px 30px;
    display: flex;
    flex-direction: column;
    position: relative;
    z-index: 500;
  }
</style>
