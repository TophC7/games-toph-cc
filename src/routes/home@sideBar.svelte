<script>
	import Fa from 'svelte-fa';
	import { faChevronRight, faHashtag, faFaceLaugh, faPlus } from '@fortawesome/free-solid-svg-icons';
	import Astronaut from '../../static/astronaut.svelte';
	import Post from '../components/post.svelte';
</script>

<div class="flex bg-primary h-screen font-baloo">
	<!-- INFO: column with titles and lists -->
	<div name="first-col" class="flex flex-col w-1/4 min-w-max z-40 px-4 gap-4 shadow-xl">
		<header class="flex h-24 place-items-center mb-1">
			<p class="font-black text-4xl text-offWhite mt-1">Welcome</p>
		</header>

		<div class="flex text-3xl gap-4 place-items-center font-semibold text-complementary">
			<Fa icon={faChevronRight} />
			<p class="mt-1 text-grayAccent">About me🧍🏽</p>
		</div>
		<!-- <div class="w-2/3 border-2 mx-auto rounded-sm border-secondary bg-secondary" /> -->
	</div>

	<!-- INFO: column with content -->
	<div name="second-col" class="flex mt-24 w-3/4 bg-secondary z-30">
		<header class="fixed top-0 flex h-24 w-full p-4 text-4xl gap-4 place-items-center font-semibold  text-grayAccent bg-secondary shadow-xl">
			<Fa icon={faHashtag} />
			<p class=" mt-1 text-complementary">Hello</p>
		</header>
		<div class="flex flex-col pt-6 pl-6 h-full w-24 min-w-max">
			<i class="avatar">
				<Astronaut color="currentColor" opacity="0.5" />
			</i>
		</div>
		<div class="flex flex-col p-6 h-full gap-4">
			<Post reaction={true}>
				<p>Hola</p>
			</Post>
		</div>
	</div>
</div>
