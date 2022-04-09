<script>
	import '../app.css';
	import Croissant from '../../static/croissant.svelte';
	import SpaceCat from '../../static/spaceCat.svelte';
	import Briefcase from '../../static/briefcase.svelte';
	import Notebook from '../../static/notebook.svelte';
	import Github from '../../static/github.svelte';
</script>

<div class=" ml-24">
	<nav class="fixed left-0 flex flex-col w-24 h-screen gap-4 p-3 bg-[#18171a] shadow-2xl z-50">
		<i class="sidebar-icon group">
			<Croissant color="currentColor" opacity="0.5" />
			<span class="sidebar-tooltip group-hover:scale-100"> Kwahson </span>
		</i>

		<div class="divider" />

		<i class="sidebar-icon group">
			<Notebook color="currentColor" opacity="0.5" />
			<span class="sidebar-tooltip group-hover:scale-100"> My Projects </span>
		</i>
		<i class="sidebar-icon group">
			<Briefcase color="currentColor" opacity="0.5" />
			<span class="sidebar-tooltip group-hover:scale-100"> Experience </span>
		</i>
		<i class="sidebar-icon group">
			<SpaceCat color="currentColor" opacity="0.2" />
			<span class="sidebar-tooltip group-hover:scale-100"> My Cats! </span>
		</i>

		<div class="divider" />

		<i class="sidebar-icon group">
			<Github color="currentColor" />
			<span class="sidebar-tooltip group-hover:scale-100"> Github </span>
		</i>
	</nav>

	<slot />
</div>
