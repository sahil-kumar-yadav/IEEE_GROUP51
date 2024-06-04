<script>
  import Object from "./Object.svelte";

  import ActionTitle from "./ActionTitle.svelte";

  import Actionbar from "./Actionbar.svelte";
</script>

<div class="actionBody">
  <ActionTitle />
  <div class="subtitle">Object</div>
  <Object />
  <div class="subtitle">
    Duration
    <div class="durationInput">
      <div class="durationText">
        <input placeholder="0.6" class="outlinedInput" />
      </div>
      <div class="durationType">
        <div class="dropdownWrapper">
          <div class="currentDropdownItem">
            <span class="dropdownItemName">s </span>
            <span class="arrowDown">▼</span>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="subtitle">
    Timing Function
    <div class="timingFunction">
      <div class="dropdownWrapper">
        <div class="currentDropdownItem">
          <span class="dropdownItemName">linear </span>
          <span class="arrowDown">▼</span>
        </div>
      </div>
    </div>
  </div>
  <div class="subtitle">
    Delay
    <div class="durationInput">
      <div class="durationText">
        <input class="outlinedInput" />
      </div>
      <div class="durationType">
        <div class="dropdownWrapper">
          <div class="currentDropdownItem">
            <span class="dropdownItemName">s </span>
            <span class="arrowDown">▼</span>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="subtitle">
    <span>Iteration</span>
    <label for="" class="infiniteCheckboxTitle"> Infinite</label>
    <br />
    <div class="durationInput">
      <div class="durationText">
        <input class="outlinedInput" />
      </div>
      <div class="durationType">
        <input style="vertical-align: middle;" type="checkbox" />
      </div>
    </div>
  </div>
  <div class="subtitle">
    Direction
    <div class="timingFunction">
      <div class="dropdownWrapper">
        <div class="currentDropdownItem">
          <span class="dropdownItemName">normal </span>
          <span class="arrowDown">▼</span>
        </div>
      </div>
    </div>
  </div>
  <div class="subtitle actionBtnWrap centered">
    <a href=" " class="actionButton">Animations</a>
  </div>
</div>

<style>
  .actionBody {
    width: 85%;
    position: absolute;
  }
  .subtitle {
    font-family: "Poppins";
    color: black;
    font-weight: 900;
    font-size: 12px;
    line-height: 20px;
    margin-top: 15px;
  }
  .durationInput {
    display: flex;
    align-items: center;
    height: 30px;
  }
  .durationText {
    height: 100%;
    width: 70%;
    margin-right: 5px;
  }
  .outlinedInput {
    outline: 0;
    border: 2px solid #e4e1f0;
    padding: 5px;
    border-radius: 4px;
    width: 100%;
    height: 100%;
    font-family: "Poppins";
    font-weight: 700;
    color: #87868b;
    box-sizing: border-box;
  }
  .durationType {
    height: 100%;
    width: 20%;
    display: flex;
    align-items: center;
  }
  .infiniteCheckboxTitle {
    position: absolute;
    right: 30px;
  }
  .centered {
    text-align: center;
    /* font-family: "Poppins";
    color: #a19bbb;
    font-weight: 900;
    font-size: 12px;
    line-height: 20px; */
  }
  .dropdownWrapper {
    pointer-events: auto;
    width: 100%;
    height: 100%;
    position: relative;
    box-sizing: border-box;
  }
  .currentDropdownItem {
    border: 2px solid #e4e1f0;
    border-radius: 4px;
    font-weight: 700;
    padding-left: 3px;
    font-family: "Poppins";
    cursor: pointer;
    display: flex;
    justify-content: space-between;
    /* jbjb */
    width: 100%;
    height: 100%;
    position: relative;
    box-sizing: border-box;
  }
  .dropdownItemName {
    font-size: 12px;
    display: flex;
    justify-content: center;
    align-items: center;
    padding-right: 4px;
  }
  .arrowDown {
    font-size: 12px;
    display: flex;
    justify-content: center;
    align-items: center;
    padding-right: 4px;
  }
  .timingFunction {
    height: 30px;
  }
  .actionButton {
    border: 2px solid #e4e1f0;
    padding: 10px 40px;
    border-radius: 7px;
    cursor: pointer;
    position: relative;
    z-index: 100;
  }
</style>
