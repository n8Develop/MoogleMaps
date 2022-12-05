<script>
  import HeadSearch from "/components/Heading/HeadSearch.svelte";
  import MapHolder from "/components/Map/MapHolder.svelte";
  import TableHolder from "/components/Table/TableHolder.svelte";
  import CursorHandler from "/components/Cursor/cursorHandler.svelte";
  import Footing from "/components/Footer/Footing.svelte";

  import Data from "//data.json";
</script>

<style>
  main {
    font-family: sans-serif;
    cursor: url("cursor2.png"), auto;
  }
  .flexArea {
    display: flex;
  }
</style>

<main>
	
<HeadSearch class="hds"/>
<div class="flexArea">
<TableHolder dataHold={Data} class="tbho"/>
<MapHolder class="mpho"/>
</div>
<CursorHandler class="crsr"/>
<Footing class="fting"/>

</main>