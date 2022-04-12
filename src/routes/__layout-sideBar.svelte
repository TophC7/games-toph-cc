<script>
	import '../app.css';
	import Croissant from '../../static/croissant.svelte';
	import SpaceCat from '../../static/spaceCat.svelte';
	import Briefcase from '../../static/briefcase.svelte';
	import Notebook from '../../static/notebook.svelte';
	import Github from '../../static/github.svelte';
</script>

<div class="ml-24" id="side-bar">
	<nav class="fixed left-0 flex flex-col w-24 h-screen gap-4 p-3 bg-[#18171a] shadow-2xl z-50">
		<a class="sidebar-icon group" href="/">
			<div class=" group-hover:spin">
				<Croissant color="currentColor" opacity="0.5" />
			</div>
			<span class="sidebar-tooltip group-hover:scale-100"> Kwahson </span>
		</a>

		<div class="divider" />

		<a class="sidebar-icon group" href="/projects">
			<Notebook color="currentColor" opacity="0.5" />
			<span class="sidebar-tooltip group-hover:scale-100"> My Projects </span>
		</a>
		<a class="sidebar-icon group" href="/experience">
			<Briefcase color="currentColor" opacity="0.5" />
			<span class="sidebar-tooltip group-hover:scale-100"> Experience </span>
		</a>
		<a class="sidebar-icon group" href="/cats">
			<SpaceCat color="currentColor" opacity="0.2" />
			<span class="sidebar-tooltip group-hover:scale-100"> My Cats! </span>
		</a>

		<div class="divider" />

		<a class="sidebar-icon group" href="https://github.com/TophC7">
			<Github color="currentColor" />
			<span class="sidebar-tooltip group-hover:scale-100"> Github </span>
		</a>
	</nav>

	<slot />
</div>

<style>
	@keyframes spin {
		to {
			transform: rotate(360deg);
		}
	}
	.group:hover .group-hover\:spin {
		animation: spin 1.5s linear infinite;
	}
</style>
