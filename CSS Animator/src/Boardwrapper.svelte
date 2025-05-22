<script>
  import Board from "./Board.svelte";
  import ActionBody from "./ActionBody.svelte";
</script>

<div class="boardWrapper">
  <div class="action">
    <ActionBody />
  </div>
  <Board />
</div>

<style>
  .boardWrapper {
    width: 100%;
    display: flex;
    max-height: 100%;
    /* position: relative; */
    /* background-color: rgba(69, 102, 135, 0.838); */
  }
  .action {
    background: #b4be87;
    width: 17rem;
    border-right: 1px solid black;
    max-height: 100%;
    padding: 40px 20px;
    position: relative;
  }
</style>
