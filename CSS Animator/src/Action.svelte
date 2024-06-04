<script>
  import ActionBody from './ActionBody.svelte';

  import Actionbar from "./Actionbar.svelte";
</script>

<div class="action">
  <div style="opacity: 1;">
    <div>
      <ActionBody></ActionBody>
    </div>
  </div>
</div>

<style>
  .action {
    width: 15rem;
    border-right: 1px solid black;
    max-height: 100%;
    padding: 40px 20px;
    position: relative;
    /* height: 100%; */
    height: 86%;
  }
</style>
