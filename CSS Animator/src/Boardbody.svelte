<script>
  import Animation from "./Animation.svelte";

  import Boardhead from "./Boardhead.svelte";

  import Action from "./Action.svelte";

  import Actionbar from "./Actionbar.svelte";
</script>

<div class="boardBody">
  <Animation />
  <div
    style="transform: scale(1); opacity: 1;"
    id="objectSquare"
    class="objectSquare"
  />
</div>

<style>
  .boardBody {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
    width: 100%;
    position: relative;
  }
  .objectSquare {
    position: absolute;
    width: 150px;
    height: 150px;
    /* width: 200px;
    height: 200px; */
    background-color: #FFA5A5;
    border-radius: 10px;
  }
</style>
