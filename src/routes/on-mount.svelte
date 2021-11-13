<script lang="ts">
	let colour = 'blue';
	import { onMount } from 'svelte';
	onMount(() => {
		setTimeout(() => {
			colour = 'green';
		}, 3000);
		colour = 'red';
	});
</script>

<div style="background-color: {colour}">
	This div should be blue if the component is server rendered or red in the browser, and change to
	green after 3 seconds.
</div>
