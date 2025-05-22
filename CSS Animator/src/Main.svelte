<script>
  import Boardwrapper from './Boardwrapper.svelte';

  import Actionbar from './Actionbar.svelte';

</script>

<div class="main">
        <Actionbar></Actionbar>
        <Boardwrapper></Boardwrapper>
      </div>

<style>
  .main {
  height: 91vh;
  display: flex;
  flex-direction: row;
}
</style>

