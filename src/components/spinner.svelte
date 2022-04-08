<div id="spinner">
	<div id="spinner-inside">
		<span id="left-span" /> <span id="right-span" />
	</div>
</div>

<style>
	#spinner {
		display: flex;
		height: 5rem;
		width: 5rem;
		color: #fff;
		border: 5px solid;
		border-radius: 50%;
		border-top-color: transparent;
		animation: rotate 1s linear infinite;
		align-items: center;
		justify-content: center;
	}

	#spinner-inside {
		height: 100%;
		widows: 100%;
		display: flex;
		align-items: center;
		animation: rotate 0.5s linear infinite reverse;
	}

	#left-span {
		height: 40%;
		width: 1rem;
		border-top: 5px #fff solid;
		border-right: 2.5px #fff solid;
	}
	#right-span {
		height: 40%;
		width: 1rem;
		border-top: 5px #fff solid;
		border-left: 2.5px #fff solid;
	}

	@keyframes rotate {
		0% {
			transform: rotate(0);
		}
		100% {
			transform: rotate(360deg);
		}
	}
</style>
