<!DOCTYPE html>
<html lang="zh">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<meta http-equiv="X-UA-Compatible" content="ie=edge">
	<link rel="stylesheet" href="./node_modules/bootstrap/dist/css/bootstrap.min.css">
	<script src="../vue.js"></script>
	<title>指令</title>
</head>
<body>
	<div class="app">
		{{msg}}
		<div v-text="msg" class="bg-info">sdsd</div>
		<input type="text" v-model="msg">
		<div v-html="content"></div>
		<div v-if="num>1">大于一</div>
		<div v-else="num < 1">小于一</div>
	</div>
</body>
<script>
	const app = new Vue({
		el:".app",
		data:{
			msg:"1111",
			content:`<h1>aaaaaaa</h1>`,
			num:1,
		}
	})
</script>
</html>