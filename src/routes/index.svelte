<script>
	import Fa from 'svelte-fa';
	import { faChevronRight, faHashtag } from '@fortawesome/free-solid-svg-icons';
</script>

<div class="flex bg-primary h-screen font-baloo">
	<div name="first-col" class="flex flex-col w-1/4 min-w-max z-40 px-4 gap-4">
		<header class="flex h-24 place-items-center mb-1">
			<p class="font-black text-4xl text-offWhite mt-1">Welcome</p>
		</header>

		<div class="flex text-3xl gap-4 place-items-center font-semibold text-complementary">
			<Fa icon={faChevronRight} />
			<p class="mt-1 text-grayAccent">About me🧍🏽</p>
		</div>
		<!-- <div class="w-2/3 border-2 mx-auto rounded-sm border-secondary bg-secondary" /> -->
	</div>

	<div name="second-col" class="w-3/4 bg-secondary z-30">
		<header
			class="flex h-24 p-4 text-4xl gap-4 place-items-center font-semibold shadow-2xl text-grayAccent"
		>
			<Fa icon={faHashtag} />
			<p class=" mt-1 text-complementary">Hello</p>
		</header>
	</div>
</div>
