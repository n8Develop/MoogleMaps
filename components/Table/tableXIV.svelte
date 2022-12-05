<script>
import TRXIV from "./trXIV.svelte";
import MatsArray from "./matsArray.svelte";
export let dataTab;
</script>

<style>
  td {
    border: 1px solid;
  }
  table {
    background-color: #aed;
  }

  thead {
    background-color: #333;
    color: #fff;
  }
</style>
{#each dataTab as Data}
<MatsArray mats={Data.mats}/>
{/each}
<table> 
	<thead>
  <tr>
  <td>Crafted Item Table</td>
  </tr>
		<tr>
			<th>Picture</th>
        <th>Material Name</th>
        <th># required</th>
		<tr>
	</thead>
  <tbody>
  {#each dataTab as Data}
    <TRXIV {...Data}/>
    {/each}
    <tbody>
</table>



<!--I want to clickable rows containing all the mats of the crafted
item, to do so, I will try creating hidden rows attached in the
TRXIV area
-->