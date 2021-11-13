<script lang="ts">
	let colour = 'blue';
	import { browser } from '$app/env';
	debugger;
	if (browser) {
		colour = 'red';
	}
</script>

<div style="background-color: {colour}">
	This div should be blue if the component is server rendered or red in the browser.
</div>
