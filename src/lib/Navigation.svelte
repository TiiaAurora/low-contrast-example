<script>
	import { browser } from '$app/env';

	function addLowContrast() {
		document.body.classList.add('lowcontrast');
	}

	function removeLowContrast() {
		document.body.classList.remove('lowcontrast');
	}
</script>

<div class="flex items-center justify-between">
	<div>
		<a href="/" class="border-2 p-1 px-2 rounded">Text</a>
		<a href="/image" class="border-2 p-1 px-2 rounded">Images and Colours</a>
	</div>
	<div>
		<button class="border-2 p-1 px-2 rounded" on:click={addLowContrast}>Low Contrast</button>
		<button class="border-2 p-1 px-2 rounded" on:click={removeLowContrast}>High Contrast</button>
	</div>
</div>
