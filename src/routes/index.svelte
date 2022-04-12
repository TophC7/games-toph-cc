<script>
	import { onMount } from 'svelte';
	import Croissant from '../../static/croissant.svelte';

	onMount(async () => {
		setTimeout(() => {
			window.location.href = '/home';
			window.clearTimeout();
		}, 3000);
	});
</script>

<div class="flex flex-col w-screen h-screen bg-tertiary text-accent justify-center place-items-center gap-6" id="loading-screen">
	<span class=" w-40 h-40 spin">
		<Croissant color="currentColor" opacity="0.5" />
	</span>
	<p class="font-black font-baloo text-offWhite">Spinning the croissant...</p>
</div>

<style>
	.spin {
		animation: rotate 2s linear infinite;
	}

	@keyframes rotate {
		to {
			transform: rotate(360deg);
		}
	}
</style>
