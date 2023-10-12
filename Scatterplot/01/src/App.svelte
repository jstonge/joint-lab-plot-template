<!-- examples borrowed from: https://svelte.dev/examples/scatterplot -->

<script>
	import Scatterplot from '$components/Scatterplot.svelte';
	import data from '$data/data.js';
</script>

<div class="chart">
	<h1>Anscombe's quartet</h1>

	<Scatterplot points={data.a} />
	<Scatterplot points={data.b} />
	<Scatterplot points={data.c} />
	<Scatterplot points={data.d} />
</div>

<style>
  h1 {
    margin-top: 100px;
    margin-bottom: 100px;
    text-align: center;
    font-size: 2em;
    font-family: 'Times New Roman', Times, serif;
  }
	.chart {
		width: 100%;
		max-width: 640px;
		height: calc(100% - 4em);
		min-height: 280px;
		max-height: 480px;
		margin: 0 auto;
	}
</style>
