<template>
	<div class="container">
		<div class="navigation">
			<div class="data">
				<input type="date" placeholder="2023-01-05">
			</div>
			<input class="search" type="text" placeholder="Поиск">
		</div>
		<div class="results">
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
			<div>1</div>
		</div>

	</div>

</template>

<script>
	
</script>

<style>
	* {
		box-sizing: border-box;
	}
	.container {
/*		outline: 2px solid green;*/
		margin: 0 auto;
		width: 100%;
		height: 100vh;

		padding: 10px 64px;
		
	}
	.navigation {
		width: 100%;
		display: flex;
		
		flex-direction: row;
		justify-content: space-between;

	}

	.data {
/*		outline: 2px solid red;*/
		width: 430px;
		height: 48px;
		align-items: left;
		border-radius: 12px;
	}
	.search {
		width: 300px;
		height: 48px;
		border-radius: 12px;
	}

	.results {
		display: flex;
/*		outline: 2px solid blue;*/
		height: 276px;
		width: 100%;
		flex-direction: row;
		overflow: hidden;
		flex-wrap: wrap;
	}

	.results>div {
		width: 63px;
		height: 96px;
		outline: 1px solid black;
	}

	.results div:nth-child(4n+4) {
    color: #f00;
    margin-right: 16px;
}

	
</style>