<!doctype html>
<html lang="en">
<head>
	<meta charset="UTF-8" />
	<title>属性样式</title>
	<link rel="stylesheet" href="./node_modules/bootstrap/dist/css/bootstrap.min.css">
	<script src="../vue.js"></script>
	<style type="text/css">
			.one{

				height: 55px;
				background-color: red;
				width: 500px;
				height: 100px;
			}
			.two{
				border-radius: 20px;
				background: red;
			}
	</style>
</head>
<body>
	<div id="app" class="container">
		<div v-bind:class="{one:flag,two:flag1}">{{msg}}</div>
		<div v-bind:style="{background:'#c00'}">{{msg}}</div>
	</div
	
</body>
<script>
	let app  = new Vue({
		el:"#app",
		data:{
			msg:"hefdff",
			flag:false,
			flag1:true
			
		}
	})
	
</script>
</html>