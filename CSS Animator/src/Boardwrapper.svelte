<script>
  import Width from "./Width.svelte";

  import Actionbar from "./Actionbar.svelte";
</script>

<div class="boardWrapper">
  <Width />
</div>

<style>
  .boardWrapper {
  width: 100%;
  /* height: 100%; */
  display: flex;
  max-height: 100%;
  position: relative;
  background-color: rgba(30, 143, 255, 0.838);
}
</style>
