<script>
  import Zoombtns from "./Zoombtns.svelte";

 
</script>

<div class="boardHead">
  <Zoombtns />
  <div class="exportBtns" style="opacity: 1;">
    <a href=" " class="primaryButton">Export</a>
  </div>  
</div>

<style>
  .boardHead {
    display: flex;
    padding: 30px;
    justify-content: space-between;
  }
  .primaryButton {
  font-family: "Poppins";
  background-color: midnightblue;
  color: #fff;
  font-weight: 700;
  padding: 10px 40px;
  border-radius: 7px;
  cursor: pointer;
  text-decoration: none;
}
</style>
