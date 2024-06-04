<script>
  import Actionbarfooter from "./Actionbarfooter.svelte";

  import Actionbarbody from "./Actionbarbody.svelte";

  import Actionbartop from "./Actionbartop.svelte";
</script>

<div class="actionBar">
  <Actionbartop />
  <Actionbarbody />
  <Actionbarfooter />
</div>

<style>
  .actionBar {
    width: 90px;
    /* background-color: #cfc860; */
    background-color: midnightblue;
    flex-direction: column;
    position: relative;
    z-index: 1000;
    height: 92vh;
    /* height: 100vh; */
    display: flex;
  }
</style>
