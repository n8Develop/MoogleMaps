<script>
	export let mats;
	let totalMats = [];
	function addToArray(props) {
	  totalMats = [...totalMats, props];
	}
</script>


<style>
</style>

{#each mats as adders}
<p class="arrayP">
{adders.join(" ")}
</p>

{/each}

