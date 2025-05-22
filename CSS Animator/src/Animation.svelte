<script>
  import Animationswrapper from "./Animationswrapper.svelte";

  import Carwrapper from "./Carwrapper.svelte";
</script>

<div class="animations" style="opacity: 1;">
  <div class="animations">
    <Carwrapper />
    <Animationswrapper />
  </div>
</div>

<style>
  .animations {
    display: flex;
    justify-content: center;
    position: absolute;
    top: 0;
  }
</style>
