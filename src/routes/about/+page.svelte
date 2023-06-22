<svelte:head>
	<title>Profile</title>
</svelte:head>

<style>
	ul {
        font: 14px Verdana, Geneva, sans-serif;
		color: #fff;
	}
    .left {
        float: left;
    }
	.main {
		color: black;
		display: inline-block;
		border: 1px solid black;
		height: 258px;
		width: 370px;
	}
	.container {
		color: black;
		border: 1px solid black;
		height: 258px;
		width: 20%;
		min-width: 258px;
		display: inline-block;
	}
	h1 {
		text-align: center;
	}
	.wrapper {
		display: table-cell;
		display: flex;
		justify-content: center;
		align-items: center;
	}
	.user {
		width: 200px;/*размер иконки по ширине*/
		height: 200px;/*размер иконки по высоте*/
		border: 24px solid gray;/*толщина и цвет рамки*/
		border-radius: 50%;/*скругление рамки */
		position: relative;/*родитель, относительно которого позиционированы псевдоэлементы*/
		overflow: hidden;/*скрывает дочерние элементы, выходящие за рамки контейнера*/
		background-color: gray;
	}
	.user::before {
		content : '';/*обязательное свойство для before*/
		display: block;
		width: 75px;/*ширина головы иконки*/
		height: 75px;/*высота головы иконки*/
		background: #fff;/*цвет*/
		border-radius: 50%;/*скругление */
		position: absolute;/*абсолютное позиционирование*/
		left: 50%;/*сдвиг от левого края родителя*/
		top: 5px;/*сдвиг вниз от верхнего края родителя*/
		transform: translateX(-50%);
	}
	.user::after {
		content : '';
		display: block;
		width: 150px;
		height: 150px;
		background: #fff;
		border-radius: 50%;
		position: absolute;
		left: 50%;
		bottom: -80px;
		transform: translateX(-50%);
	}
</style>
<ul>
<li class="left"><div class="container">
	<div class="wrapper">
		<div class="user"></div>
	</div>
	<h1>Visitor: 1</h1>
</div></li>
<li class="left">
	<div class="main">
		<h1>Unknown</h1>
		<p>Age: none,</p>
		<p>Project: 2,</p>
		<p>Reviews: no,</p>
		<p>Comments: no,</p>
		<p>Scheduled tasks: none,</p>
		<p>Completed tasks: 0.</p>
	</div>
</li>
</ul>