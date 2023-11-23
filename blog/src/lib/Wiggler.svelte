<script>
</script>

<span class="boop">
  <button>Wiggle</button>
</span>

<style>
  @keyframes boop {
    0% {
      transform: rotate(0deg);
    }
    20% {
      transform: rotate(-15deg);
    }
    40% {
      transform: rotate(15deg);
    }
    60% {
      transform: rotate(-7deg);
    }
    80% {
      transform: rotate(7deg);
    }
    90% {
      transform: rotate(-3deg);
    }
    95% {
      transform: rotate(2deg);
    }
    100% {
      transform: rotate(0deg);
    }
  }
  .boop:hover {
    display: inline-block;
    animation: 0.5s boop forwards running;
  }
</style>
