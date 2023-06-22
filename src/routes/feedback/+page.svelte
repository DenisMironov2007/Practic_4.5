<svelte:head>
	<title>Feedback</title>
</svelte:head>

<style>
	.container {
		width: 100%;
		border: 1px solid black;
		height: 200px;
		background-color: #eee;
	}
	h1 {
		border: 1px solid black;
		color: red;
	}
	.iner {
		text-align: center;
	}
	table {
		border: 3px solid black;
		position: fixed;
		bottom: 0;
		left: 0;
	}
	td {
		cursor: pointer;
	}
</style>

<div class="container">
	<h2>Reviews:</h2>
	<div class="iner">
		<h1>The site does not have reviews yet, as it is under development.</h1>
		<p>It will be published in Beta testing soon</p>
	</div>
	<table>
		<tr>
			<td>Pages: 1</td>
			<td>2</td>
			<td>3</td>
			<td>4</td>
			<td>5</td>
			<td>6</td>
		</tr>
	</table>
</div>