<script>
  import Boardhead from "./Boardhead.svelte";

  import Action from "./Action.svelte";

  import Actionbar from "./Actionbar.svelte";
</script>

<div class="carWrapper" style="transform: translateY(0px) translateZ(0px);">
  <!-- <img class="car" src="/static/media/dragon.0a5a1b10.png" alt="dragon" /> -->
</div>

<style>
  .carWrapper {
    position: absolute;
    z-index: 100;
    top: -40px;
  }
</style>
