<script>
	import Spinner from '../components/tripleSpinner.svelte';
</script>

<nav id="navbar">
	<div class="flex-middle" id="toph">
		<a class="nav-link font-baloo2" href="/"> Toph </a>
	</div>
	<div class="flex-middle" id="projects">
		<a class="nav-link font-baloo2" href="/"> Projects </a>
	</div>
	<div class="flex-middle" id="experience">
		<a class="nav-link font-baloo2" href="/"> Experience </a>
	</div>
</nav>

<div id="bg-spinner">
	<Spinner color="#000" colorSecondary="#000" spinnerSize="350px" />
</div>

<style>
	#navbar {
		display: flex;
		position: fixed;
		height: 4rem;

		/* INFO: these two basically give it its width */
		left: 0;
		right: 0;
		/* ^^ */

		z-index: 100;
	}

	#navbar div {
		padding-left: 1rem;
		padding-right: 1rem;
	}

	#toph {
		background-color: hsl(0, 0%, 100%);
		width: 100%;
	}

	#projects {
		background-color: hsl(0, 0%, 80%);
	}

	#experience {
		background-color: hsl(0, 0%, 60%);
	}

	.nav-link,
	.nav-link:any-link {
		font-weight: 700;
		font-size: 2rem;
		line-height: 2rem;
		text-decoration: none;
		color: black;
	}

	#bg-spinner {
		position: absolute;
		bottom: -9rem;
		right: -9rem;
		z-index: 0;
	}
</style>
