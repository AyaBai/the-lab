<template>
	<div>Хламидиоз  (трахоматис)</div>
		<div class="results" v-for="item in items" :key="item.number">
			
			{{ items }}
			
			</div>


			
			<div>
				<span class="number">01</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>

			<div>
			<span class="number">02</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>

			<div>
			<span class="number">05</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>

			<div>
			<span class="number">07</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>

			<div>
			<span class="number">10</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>

			<div>
			<span class="number">12</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>

			<div>
			<span class="number">16</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>
			<div>
			<span class="number">22</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>
			<div>
			<span class="number">26</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>
			<div>
			<span class="number">36</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>
			<div>
			<span class="number">39</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>
			<div>
			<span class="number">40</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>
			<div>
			<span class="number">55</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>
			<div>
			<span class="number">56</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>
			<div>
			<span class="number">59</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>
			<div>
			<span class="number">85</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>
			<div>
			<span class="number">99</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>
			<div>
			<span class="number">102</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>
			<div>
			<span class="number">107</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>
			<div>
			<span class="number">108</span><br>
				<span class="person_data_result">_.___</span><br>
				<span class="person_data">мужской</span><br>
				<span class="person_data">26 лет</span>
			</div>
		
	

</template>


<script>
	export default {
	data() {
		return {
			items: [
				{
			number:['01','02'],
				result:'',
				gender:'',	
				age:''
				}
			]
		}
	}
}
	
</script>

<style>
	.results {
		display: flex;
		outline: 2px solid blue;
		height: 276px;
		width: 100%;
		flex-direction: row;
		overflow: hidden;
		flex-wrap: wrap;
		margin-left: 70px;
		padding: 5px;

	}

</style>