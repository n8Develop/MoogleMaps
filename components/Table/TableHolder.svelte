<script>
import TableXIV from "./tableXIV.svelte";
export let dataHold;
</script>

<style>
  .tableHold {
    background-color: grey;
    width: 50%;
    border: double;
  }
</style>

<div class="tableHold">
<TableXIV dataTab={dataHold}/>
</div>