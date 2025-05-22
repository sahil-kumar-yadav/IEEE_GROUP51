<script>
    import Header from "./lib/Header.svelte";
    import MainContent from "./lib/MainContent.svelte";
    import Sidebar from "./lib/Sidebar.svelte";



  let duration = 0.6;
  let timingFunction = 'linear';
  let delay = 0;
  let iterations = 'infinite';
  let direction = 'normal';

  let animationClass = "";

const applyAnimation = (type) => {
    animationClass = "";
    setTimeout(() => {
        switch (type) {
            case "rotate":
                animationClass = "rotate";
                break;
            case "flip":
                animationClass = "flip";
                break;
            case "slide":
                animationClass = "slide";
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

<style>
  .container {
      display: flex;
      flex-direction: column;
      height: 100vh;
  }
  .content {
      display: flex;
      flex: 1;
  }
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
        from { transform: rotate(0deg); }
        to { transform: rotate(360deg); }
    }
    @keyframes flip-animation {
        from { transform: rotateY(0); }
        to { transform: rotateY(180deg); }
    }
    @keyframes slide-animation {
        from { transform: translateX(0); }
        to { transform: translateX(100px); }
    }
</style>

<div class="container">
  <Header title="Developerstar Animations" />
  <div class="content">
      <Sidebar
          {duration}
          {timingFunction}
          {delay}
          {iterations}
          {direction}
          {applyAnimation}
      />
      <MainContent {animationClass} {animationStyle} />
  </div>
</div>
