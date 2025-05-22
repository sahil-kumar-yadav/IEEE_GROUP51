<script>
</script>

<div class="animationsWrapper">
  <svg
    id="Layer_1"
    x="0px"
    y="0px"
    viewBox="0 0 492 492"
    xml:space="preserve"
    class="animationsCloseIcon"
    ><g><g /></g><g /><g /><g /><g /><g /><g /><g /><g /><g /><g /><g /><g /><g
    /><g /><g /></svg
  >
  <div
    class="swiper-container swiper-container-initialized swiper-container-horizontal"
  >
    <div class="swiper-wrapper">
      <div
        class="animationItem animationCategory swiper-slide swiper-slide-active"
        style="margin-right: 10px;"
      >
        Rotations
      </div>
      <div
        class="animationItem animationCategory swiper-slide swiper-slide-next"
        style="margin-right: 10px;"
      >
        Rotations 2
      </div>
      <div
        class="animationItem animationCategory swiper-slide"
        style="margin-right: 10px;"
      >
        Flip
      </div>
      <div
        class="animationItem animationCategory swiper-slide"
        style="margin-right: 10px;"
      >
        Flip 2
      </div>
      <div
        class="animationItem animationCategory swiper-slide"
        style="margin-right: 10px;"
      >
        Slide
      </div>
      <div
        class="animationItem animationCategory swiper-slide"
        style="margin-right: 10px;"
      >
        Slide-2
      </div>
    </div>
  </div>
</div>

<style>
  .animationsWrapper {
    background-color: #fff !important;
    height: 90px;
    min-width: 400px;
    max-width: 900px;
    border-radius: 10px;
    box-shadow: -2px 3px 12px -5px #e2e2e2;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    z-index: 1000;
    border: 4px solid black;
  }
  .animationsCloseIcon {
    width: 14px;
    height: 14px;
    fill: "black";
    position: absolute;
    top: 7px;
    right: 20px;
    z-index: 200;
    cursor: pointer;
  }

  .swiper-container {
    margin-left: auto;
    margin-right: auto;
    position: relative;
    overflow: hidden;
    list-style: none;
    padding: 0;
    z-index: 1;
  }

  .swiper-wrapper {
    position: relative;
    width: 100%;
    height: 100%;
    z-index: 1;
    display: flex;
    transition-property: transform;
    box-sizing: content-box;
  }

  .animationItem {
    /* width: -webkit-fit-content;
    width: -moz-fit-content; */
    /* width: fit-content; */
    width: max-content;
    height: 40px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #d6d4de;
    font-family: "Poppins";
    color: #282828;
    font-weight: 600;
    border-radius: 10px;
    cursor: pointer;
    font-size: 14px;
    padding: 0 20px;
    position: relative;
    /* margin-right: 10px; */
  }
</style>
