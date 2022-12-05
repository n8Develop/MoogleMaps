<script>
	export let picture = ";(";
	export let mats = "friend";
	export let quant = "99";
	export let craft = "generic";


	let visible = { hidden: false };

	function toggle() {
	  visible.hidden = !visible.hidden;
	}
</script>

<style>
  tr {
    background-color: #bae;
  }
  .pic {
  }
  .mat {
  }
  .qtn {
  }
  .craft {
  }
</style>


    <tr class="craftedRow" on:click={toggle}>
        <td class="pic">{picture}</td>
        <td class="craft">{craft}</td>
        <td class="qtn">{quant}</td>
    </tr>
    
    
    {#if visible.hidden}
        {#each mats as mat}
          <tr class="hiddenRow">
            {#each mat as index}
              <td>
                 {index}
              </td>
            {/each}
          </tr>
          
        {/each}
    {/if}

   
 