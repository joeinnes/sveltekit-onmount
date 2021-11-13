<script lang="ts">
	let colour = 'blue';
	import { browser } from '$app/env';
	debugger;
	if (browser) {
		colour = 'red';
		setTimeout(() => {
			colour = 'green';
		}, 3000);
	}
</script>

<div style="background-color: {colour}">
	This div should be blue if the component is server rendered or red in the browser, and change to
	green after 3 seconds.
</div>
