<script>
let m = { x: 0, y: 0 };
</script>

<style>
</style>


<!--In some frameworks you may see recommendations to avoid inline event handlers for performance reasons,
 particularly inside loops. That advice doesn't apply to Svelte — 
the compiler will always do the right thing, whichever form you choose.-->
<div on:mousemove="{e => m = { x:  e.clientX, y: e.clientY}}">
The mouse position is {m.x} x {m.y}
</div>