<script>
    export let duration;
    export let timingFunction;
    export let delay;
    export let iterations;
    export let direction;
    export let applyAnimation;

    let functions = ["linear", "ease", "ease-in", "ease-out", "ease-in-out"];
    let directions = ["normal", "reverse", "alternate", "alternate-reverse"];
</script>

<div class="sidebar flex">
    <h2 class="title">Create</h2>
    <div class="flex-col">
        <div >
            <label for="duration">Duration</label>
            <input
                class="input"
                type="number"
                id="duration"
                bind:value={duration}
                step="0.1"
                min="0.1"
            />
        </div>
        <div >
            <label for="timingFunction">Timing Function</label>
            <select class="input" id="timingFunction" bind:value={timingFunction}>
                {#each functions as func}
                    <option value={func}>{func}</option>
                {/each}
            </select>
        </div>
        <div >
            <label for="delay">Delay</label>
            <input
                class="input"
                type="number"
                id="delay"
                bind:value={delay}
                step="0.1"
                min="0"
            />
        </div>
        <div >
            <label for="iterations">Iteration</label>
            <input class="input" type="text" id="iterations" bind:value={iterations} />
        </div>
        <div >
            <label for="direction">Direction</label>
            <select class="input" id="direction" bind:value={direction}>
                {#each directions as dir}
                    <option value={dir}>{dir}</option>
                {/each}
            </select>
        </div>
    </div>
    
</div>

<style>
    .sidebar {
        display: flex;
        flex-direction: column;
        gap: 50px;
        background-color: wheat;
        padding: 20px;
        width: 200px;
        flex-shrink: 0;
    }
    button {
        display: block;
        margin: 5px 0;
    }
    .flex {
        display: flex;
    }
    .flex-col {
        display: flex;
        flex-direction: column;
        gap: 10px;
    }
    .input {
        margin-top: 4px;
        outline: 0;
        border: 2px solid #e4e1f0;
        padding: 5px;
        border-radius: 4px;
        width: 100%;
        height: 55%;
        font-family: "Poppins";
        font-weight: 700;
        /* color: #87868b; */
        box-sizing: border-box;
    }
    
</style>
