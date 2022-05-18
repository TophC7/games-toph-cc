<script>
	// import Fa from 'svelte-fa';
	// import { faFaceLaugh } from '@fortawesome/free-solid-svg-icons';

	export var reaction = false;
</script>

<div class=" flex flex-col relative max-w-max rounded-xl p-6 bg-grayAccent text-tertiary text-2xl gap-4 shadow-lg">
	<slot />

	{#if reaction == true}
		<!-- FIXME: this should be a button that adds up rn does nothing !!! -->
		<div class="flex absolute text-grayAccent h-6 gap-2 -bottom-8 right-0 justify-center place-items-center">
			<span class="flex bg-grayAccent h-5 w-full p-1 rounded text-sm text-complementary place-items-center font-bold"> 12 </span>
			<!-- <Fa icon={faFaceLaugh} /> -->
			<!-- <i class="absolute -top-4 -right-4"> <Fa icon={faPlus} scale={0.6} /> </i> -->
		</div>
	{/if}
</div>
