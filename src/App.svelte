<script>
	import Chart from './Chart.svelte'

	let labels = ['Marco', 'James', 'Xavier', 'Pordz', 'Awjay', 'Barry Allen']
	let data = [1,2,3,4,5,6]
	let label = "# of Votes"

</script>

<div class="input-score">
	<div class="score">
		<label for="marco">Marco</label>
		<input type="number" bind:value={data[0]} name="marco">
	</div>
	<div class="score">
		<label for="allen">James</label>
		<input type="number" bind:value={data[1]} name="allen">
	</div>
	<div class="score">
		<label for="xavier">Xavier</label>
		<input type="number" bind:value={data[2]} name="xavier">
	</div>
	<div class="score">
		<label for="awjay">Pordz</label>
		<input type="number" bind:value={data[3]} name="awjay">
	</div>
	<div class="score">
		<label for="fordi">Awjay</label>
		<input type="number" bind:value={data[4]} name="fordi">
	</div>
	<div class="score">
		<label for="jamezz">Barry Allen</label>
		<input type="number" bind:value={data[5]} name="jamezz">
	</div>
</div>


<Chart data={data} labels={labels} label={label}/>


<style>
.input-score {
	display: flex;
	flex-direction: row;
	gap: 5px;
}
.input-score > div
{
    flex:1 1 auto;
    text-align:center;
    margin:5px; 
}
</style>