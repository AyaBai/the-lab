<link rel="stylesheet" href="https://meyerweb.com/eric/tools/css/reset/reset.css">
<link rel="stylesheet" href="./fonts/stylesheet.css">
<template>
	<NavBar></NavBar>
	<div class="container">
		<DateSearch></DateSearch>
		<div class="result_container">
			<LeftMenu></LeftMenu>
			<ResultCell></ResultCell>
		</div>
	</div>

</template>

<script>

	import NavBar from './components/NavBar.vue'
	import DateSearch from './components/DateSearch.vue'
	import LeftMenu from './components/LeftMenu.vue'
	import ResultCell from './components/ResultCell.vue'
	

	export default {
		components:{
			NavBar, DateSearch, LeftMenu, ResultCell
		},

		// data() {
		// 	return {
		// 		items: [
		// 			{
		// 			number:'01',
		// 			result:'',
		// 			gender:'',	
		// 			age:''
		// 			}
		// 		]
		// 	}
		// }
	}

	
</script>

<style>
	/*@font-face {
		font-family:'SF Pro Display';
		font-style: normal;
		font-weight: 500;
		src: local("SFProDisplay-Regular"),
				url("fonts/SFProDisplay-Regular.woff2") format("woff2"),
				url("fonts/SFProDisplay-Regular.woff") format("woff");
	}
		@font-face {
		font-family:'SF Pro Display';
		font-style: normal;
		font-weight: 700;
		src: local("SFProDisplay-Black"),
				url("fonts/SFProDisplay-Black.woff2") format("woff2"),
				url("fonts/SFProDisplay-Black.woff") format("woff");
	}

	@font-face {
		font-family:'SF Pro Display';
		font-style: normal;
		font-weight: 300;
		src: local("SFProDisplay-Light"),
				url("fonts/SFProDisplay-Light.woff2") format("woff2"),
				url("fonts/SFProDisplay-Light.woff") format("woff");
	}*/


	* {
		box-sizing: border-box;
		font-family: SF Pro Display, sans-serif;
		margin: 0;
	}


	.heading {
		position: relative;
		width: 100%;
		height: 48px;
		background-color: #27272A;
		display: flex;
		flex-direction: row;
		align-items: center;
		margin-bottom: 104px;
	}

	.logo {
		width: 94px;
		height: 31px;
		background-image: url(img/Group 5110.svg);
		background-repeat: no-repeat;
		margin: 10px 0 7px 57px;
	}
	.number {
		font-weight: 700;
		font-size: 24px;
		color: #3F3F46;
		letter-spacing: 0.1px;
		padding-left: 6px;
		padding-top: 6px;
	}

	.person_data{
		font-size: 12px;
		letter-spacing: 0.4px;
		color: #52525B;
		padding-left: 6px;

	}
	.person_data_result {
		font-weight: 600;
		letter-spacing: 3.1px;
		color: #52525B;
		padding-left: 6px;
	}

	.btn_date{
		height: 44px;
		width: 100px;
		padding: 12px 19px;
		letter-spacing: 0.1px;
		color: #71717A;
		background-color: rgba(28,28,28,0);
		border: none;
		font-size: 16px;
/*		background: transparent;*/
	}

	.calendar {
		background: #0098EA;
		height: 44px;
		width: 203px;
		border-radius: 10px;
		box-shadow: 0px 1px 4px rgba(0, 131, 204, 0.33), 0px 1px 1px rgba(0, 44, 85, 0.08);
		padding: 12px 20px 12px 24px;
		border: none;
		gap: 10px;
		color: #fff;
		outline: 0;
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
/*		font-family: SF Pro Display;*/
		color: #18181B;
		font-size: 72px;
		font-weight: 500;
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

	.date {
/*		outline: 2px solid red;*/
		width: 430px;
		height: 48px;
		border-radius: 12px;
		border: 1px solid #A1A1AA;
		display: flex;
		justify-content: space-between;
	}

	.search {
		width: 581px;
		height: 48px;
		border-radius: 12px;
		border: 1px solid #A1A1AA;
		padding-left: 12px;
	}

	.input_search {
		width: 80%;
		height: 44px;
		border-radius: 12px;
		border-color: #A1A1AA ;
		border: none;
		outline: 0;

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

	.result_container {
		display: flex;
	}



	.results > div {
		width: 63px;
		height: 96px;
		border: 1px solid #D4D4D8;
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
		box-shadow: 0px 1px 4px rgba(0, 0, 0, 0.15), 0px 1px 1px rgba(0, 0, 0, 0.08);
	}

	

	.menu> div> img {
		width: 24px;
		height: 24px;
/*		outline: 2px solid red;*/
	}

	
	
</style>