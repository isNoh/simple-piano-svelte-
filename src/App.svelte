<script>
	function forTest() {
		console.log("Test!");
	}
</script>

<main>
	<h1>Simple Piano!</h1>
	<div class="piano-main">
		<div class="piano-key">
			<div on:click={forTest} class="piano-key__white">C</div>
			<div on:click={forTest} class="piano-key__black black__Db">C#/Db</div>
			<div on:click={forTest} class="piano-key__white">D</div>
			<div on:click={forTest} class="piano-key__black black__Eb">D#/Eb</div>
			<div on:click={forTest} class="piano-key__white">E</div>
			<div on:click={forTest} class="piano-key__white">F</div>
			<div on:click={forTest} class="piano-key__black black__Gb">F#/Gb</div>
			<div on:click={forTest} class="piano-key__white">G</div>
			<div on:click={forTest} class="piano-key__black black__Ab">G#/Ab</div>
			<div on:click={forTest} class="piano-key__white">A</div>
			<div on:click={forTest} class="piano-key__black black__Bb">A#/Bb</div>
			<div on:click={forTest} class="piano-key__white">B</div>
		</div>
	</div>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 100%;
		margin: 0 auto;
	}

	h1 {
		color: rgb(0, 177, 44);
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}
	.piano-main {
		margin-top: 150px;
		display: flex;
		justify-content: center;
	}
	.piano-key {
		width: 1500px;
		height: 500px;
		background-color: beige;
		display: flex;
		justify-content: space-around;
		align-items: center;
		position: relative;
		padding: 50px;
	}

	.piano-key__white {
		background-color: white;
		width: 200px;
		height: 450px;
		border: 1px solid rgba(0, 0, 0, 0.3);
		line-height: 750px;
	}

	.piano-key__black {
		background-color: black;
		width: 120px;
		height: 300px;
		color: white;
		position: absolute;
		line-height: 450px;
	}

	.black__Db {
		top: 74px;
		left: 204px;
	}

	.black__Eb {
		top: 74px;
		left: 420px;
	}

	.black__Gb {
		top: 74px;
		right: 634px;
	}

	.black__Ab {
		top: 74px;
		right: 419px;
	}

	.black__Bb {
		top: 74px;
		right: 204px;
	}
	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
