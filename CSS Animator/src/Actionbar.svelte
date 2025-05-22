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
    padding-top: 10px;
    width: 12vh;
    /* background-color: #cfc860; */
    background-color: rgb(25, 63, 112);
    display: flex;
    flex-direction: column;
    /* position: relative; */
  }
</style>
