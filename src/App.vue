<template>
	<div class="heading">
		<div class="logo"></div>
		<nav class="head_nav">
			<div>Интерпретация</div>
			<div>Клиника / Биохимия</div>
			<div>Забор материала</div>
			<div>Лабараторный журнал</div>
		</nav>

	</div>
	<div class="container">
		<p class="page_name">Интерпретация</p>
		<div class="navigation">
			<div class="btn_menu">
				<button class="btn"></button>
			

			</div>

			<div class="data">
				<button class="btn_date">Сегодня</button>
				<button class="btn_date">Вчера</button>
				<input type="date" placeholder="2023-01-05">
			</div>
			
			<div class="search">
				<img src="./img/Vector.svg" alt="">
				<input class="input_search" type="text" placeholder="Поиск">
			</div>
			
		</div>
		<div class="results">
			<div>
				<span>01</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>

			<div>
			<span>02</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>

			<div>
			<span>05</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>

			<div>
			<span>07</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>

			<div>
			<span>10</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>

			<div>
			<span>12</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>

			<div>
			<span>16</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>
			<div>
			<span>22</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>
			<div>
			<span>26</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>
			<div>
			<span>36</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>
			<div>
			<span>39</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>
			<div>
			<span>40</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>
			<div>
			<span>55</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>
			<div>
			<span>56</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>
			<div>
			<span>59</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>
			<div>
			<span>85</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>
			<div>
			<span>99</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>
			<div>
			<span>102</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>
			<div>
			<span>107</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>
			<div>
			<span>108</span><br>
				<span>_.___</span><br>
				<span>мужской</span><br>
				<span>26 лет</span>
			</div>
		</div>

	</div>

</template>

<script>
	
</script>

<style>
	@font-face {
		font-family:'SF Pro Display';
		font-style: normal;
		font-weight: 500;
		src: local("SFProDisplay-Regular"),
				url("fonts/SFProDisplay-Regular.woff2") format("woff2"),
				url("fonts/SFProDisplay-Regular.woff") format("woff");
	}
		/*@font-face {
		font-family:'SF Pro Display';
		font-style: normal;
		font-weight: 500;
		src: local("SFProDisplay-Black"),
				url("fonts/SFProDisplay-Black.woff2") format("woff2"),
				url("fonts/SFProDisplay-Black.woff") format("woff");
	}*/


	* {
		box-sizing: border-box;
		font-family: SF Pro Display;
	}

	.heading {
		position: relative;
		width: 100%;
		height: 48px;
		background-color: #27272A;
		display: flex;
		flex-direction: row;
		align-items: center;
	}

	.logo {
		width: 94px;
		height: 31px;
		background-image: url(img/Group 5110.svg);
		background-repeat: no-repeat;
		margin: 10px 0 7px 57px;
	}


	.head_nav {
		width: 745px;
		height: 48px;
		display: flex;
		flex-direction: row;
		align-items: center;
		font-size: 16px;
		color: #FFFFFF;
		justify-content: space-between;
		margin-left: 194px;
	}

	.page_name {
		font-family: SF Pro Display;
		color: #18181B;
		font-size: 72px;
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
		margin-bottom: 31px;
		flex-direction: row;
		justify-content: space-between;
		
		flex-direction: row;
	}

	.data {
		outline: 2px solid red;
		width: 430px;
		height: 48px;
		align-items: left;
		border-radius: 12px;
	}
	.search {
		width: 300px;
		height: 48px;
		border-radius: 12px;
		outline: 1px solid #A1A1AA;
		padding-left: 12px;
	}

	.input_search {
		width: 80%;
		height: 48px;
		border-radius: 12px;
		border-color: #A1A1AA ;
		border: none;

	}

	.results {
		display: flex;
/*		outline: 2px solid blue;*/
		height: 276px;
		width: 100%;
		flex-direction: row;
		overflow: hidden;
		flex-wrap: wrap;
		margin-left: 70px;
		padding: 5px;
	}

	.results>div {
		width: 63px;
		height: 96px;
		outline: 1px solid black;
		margin-right: 9px;
		border-radius: 12px;
		text-align: left;
	}

	.results div:nth-child(4n+4) {
    margin-right: 16px;
}

	.btn {
		width: 48px;
		height: 48px;
		background-color: #0098EA;
		border-color: transparent;
		border-radius: 12px;
		background-image: url(./img/format_list_bulleted_black_24dp 1.svg);
		background-repeat: no-repeat;
		background-position: center;
	}

	.btn_menu {
/*		outline: 2px solid black;*/
		width: 279px;
		height: 48px;
		border-radius: 12px;
		filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
	}
	
</style>