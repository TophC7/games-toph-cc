<script>
	export let color;
	export let colorSecondary;
	export let spinnerSize;
</script>

<div
	class="m-spinner--swirl"
	style="--color: {color}; --color-secondary: {colorSecondary}; --spinner-size: {spinnerSize}"
/>

<style>
	.m-spinner--swirl {
		--spinner-color: var(--color);
		--spinner-color-secondary: var(--color-secondary);
		--spinner-duration: 6s;
		--spinner-size: 64px;
		display: inline-flex;
		font-size: var(--spinner-size);
		color: var(--spinner-color);
		width: 1em;
		height: 1em;
		max-width: 1em;
		max-height: 1em;
		position: relative;
		animation-duration: var(--spinner-duration);
	}
	.m-spinner--swirl:before {
		top: 0.05em;
		right: 0.05em;
		bottom: 0.05em;
		left: 0.05em;
		animation-duration: 5s;
	}
	.m-spinner--swirl:after {
		top: 0.135em;
		right: 0.135em;
		bottom: 0.135em;
		left: 0.135em;
		animation-duration: 4s;
	}
	.m-spinner--swirl,
	.m-spinner--swirl:after,
	.m-spinner--swirl:before {
		border: 0.0333em solid transparent;
		border-radius: 50%;
		border-top-color: currentColor;
		border-bottom-color: currentColor;
		animation-name: m-spinner-swirl;
		animation-iteration-count: infinite;
		animation-timing-function: linear;
	}
	.m-spinner--swirl:after,
	.m-spinner--swirl:before {
		content: '';
		position: absolute;
	}
	@keyframes m-spinner-swirl {
		0% {
			transform: rotate(0deg);
		}
		50% {
			color: var(--spinner-color-secondary);
		}
		to {
			transform: rotate(1turn);
		}
	}
</style>
