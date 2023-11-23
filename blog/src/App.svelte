<script lang="ts">
  import codeEmoji from "./assets/code-emoji.svg";
  import pandaEmoji from "./assets/panda-emoji.svg";
  import climbingEmoji from "/climbing-emoji.svg";
  import Wiggler from "./lib/Wiggler.svelte";
</script>

<main>
  <div>
    <a
      href="https://www.youtube.com/watch?v=7Agd_CaHznE"
      target="_blank"
      rel="noreferrer"
    >
      <img src={climbingEmoji} class="logo" alt="Climbing Emoji" />
    </a>
    <a href="https://martinfowler.com" target="_blank" rel="noreferrer">
      <img src={codeEmoji} class="logo coding" alt="Code Emoji" />
    </a>
    <a
      href="https://en.wikipedia.org/wiki/Giant_panda"
      target="_blank"
      rel="noreferrer"
    >
      <img src={pandaEmoji} class="logo panda" alt="Panda Emoji" />
    </a>
  </div>
  <h1>Climbing + Coding + Pandas</h1>

  <div class="card">
    <Wiggler />
  </div>
</main>

<style>
  .logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
    transition: filter 300ms;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #ddff60aa);
  }
  .logo.coding:hover {
    filter: drop-shadow(0 0 2em #ff3e00aa);
  }
  .logo.panda:hover {
    filter: drop-shadow(0 0 2em #48ff00c3);
  }
</style>
