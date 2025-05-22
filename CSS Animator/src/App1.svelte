<!-- npm run dev -->
<script>
  let duration = 0.6;
  let timingFunction = "linear";
  let delay = 0;
  let iterations = "infinite";
  let direction = "normal";

  


  // 
  let animationClass = '';

    const applyAnimation = (type) => {
        animationClass = '';
        setTimeout(() => {
            switch(type) {
                case 'rotate':
                    animationClass = 'rotate';
                    break;
                case 'flip':
                    animationClass = 'flip';
                    break;
                case 'slide':
                    animationClass = 'slide';
                    break;
                // Add more cases as needed
            }
        }, 50);
    };

    $: animationStyle = `
        animation-duration: ${duration}s;
        animation-timing-function: ${timingFunction};
        animation-delay: ${delay}s;
        animation-iteration-count: ${iterations};
        animation-direction: ${direction};
    `;

    
</script>

<main>
  <div class="container">
    <div class="sidebar">
      <h2>Create</h2>
      <div>
        <label>Duration</label>
        <input type="number" bind:value={duration} step="0.1" min="0.1" />
        <label>Timing Function</label>
        <select bind:value={timingFunction}>
          <option value="linear">linear</option>
          <option value="ease">ease</option>
          <option value="ease-in">ease-in</option>
          <option value="ease-out">ease-out</option>
          <option value="ease-in-out">ease-in-out</option>
        </select>
        <label>Delay</label>
        <input type="number" bind:value={delay} step="0.1" min="0" />
        <label>Iteration</label>
        <input type="text" bind:value={iterations} />
        <label>Direction</label>
        <select bind:value={direction}>
          <option value="normal">normal</option>
          <option value="reverse">reverse</option>
          <option value="alternate">alternate</option>
          <option value="alternate-reverse">alternate-reverse</option>
        </select>
      </div>
      <button on:click={() => applyAnimation("rotate")}>Rotations</button>
      <button on:click={() => applyAnimation("rotate2")}>Rotations 2</button>
      <button on:click={() => applyAnimation("flip")}>Flip</button>
      <button on:click={() => applyAnimation("flip2")}>Flip 2</button>
      <button on:click={() => applyAnimation("slide")}>Slide</button>
      <button on:click={() => applyAnimation("slide2")}>Slide 2</button>
    </div>
    <div class="animation-controls">
      <div class="object {animationClass}" style={animationStyle}></div>
  </div>
  </div>
</main>

<style>
  .container {
    display: flex;
  }
  .sidebar {
    background-color: #a9a97b;
    padding: 20px;
    width: 200px;
  }
  .animation-controls {
    margin-left: 20px;
  }
  .object {
    width: 100px;
    height: 100px;
    background-color: pink;
  }
  /*  */
  .rotate {
    animation: rotate-animation 0.6s linear infinite;
  }
  .flip {
    animation: flip-animation 0.6s linear infinite;
  }
  .slide {
    animation: slide-animation 0.6s linear infinite;
  }

  @keyframes rotate-animation {
    from {
      transform: rotate(0deg);
    }
    to {
      transform: rotate(360deg);
    }
  }
  @keyframes flip-animation {
    from {
      transform: rotateY(0);
    }
    to {
      transform: rotateY(180deg);
    }
  }
  @keyframes slide-animation {
    from {
      transform: translateX(0);
    }
    to {
      transform: translateX(100px);
    }
  }
</style>
