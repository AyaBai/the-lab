<template>
	<div class="menu">
		<div  class="menu_2">
			<img src="../img/equalizer.svg" alt="">
		Иммуноферментные
		</div>

		<div class="line"></div>
		<div>
			<ul>
				<li>Урогенитальные инфекции</li>
				<li>Вирусные гепатиты</li>
				<li>Гельминтов</li>
				<li>Онкомаркеры</li>
				<li>Цитокины</li>
				<li>Зоонозные инфекции</li>
				<li>Гормоны</li>
				<li>Другие</li>
			</ul>
		</div>
		<div>
			<img src="../img/biotech.svg" alt="">
		Биохимические</div>
		<div class="line2"></div>
		<ul>
			<li>Биохимия</li>
			<li>ОАК</li>
			<li>ОАМ</li>
			<li>Коагулограмма</li>
		</ul>
			
		</div>

</template>


<script>
	
</script>

<style>
	.menu {
		position: relative;
		width: 426px;
		height: 569px;
		box-shadow: 0px 3.67457px 12.861px -2.75593px rgba(24, 39, 75, 0.12), 0px 8.26779px 40.4203px -1.83729px rgba(24, 39, 75, 0.14);
		font-weight: 400;
		font-size: 16px;
		letter-spacing: 0.1px;
		color: #52525B;
	}

	li {
		font-size: 14px;
	}

	.menu_2 {
		margin-bottom: 10px;
	}

	.line {
		position: absolute;
		height: 285px;
		border-left: 1px solid #E4E4E7;
		margin-right: 18px ;
    margin-left: 24px;
    display: flex;
	}

	.line2 {
		position: absolute;
		height: 141px;
		border-left: 1px solid #E4E4E7;
		margin-right: 18px ;
    margin-left: 24px;
    display: flex;
	}


/*	li:before {
		content: "";
		border-left: 6px solid green;
	}*/

	li {
		list-style: none;
		padding: 8px 26px 8px 10px;
		gap: 10px;
	}
	
	
</style>