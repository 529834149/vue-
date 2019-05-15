<!DOCTYPE html>
<html lang="zh">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<meta http-equiv="X-UA-Compatible" content="ie=edge">
	<link rel="stylesheet" href="./node_modules/bootstrap/dist/css/bootstrap.min.css">
	<script src="../vue.js"></script>
	<title>生命周期</title>
</head>
<body>
	<!--  钩子函数 -->
	<div id="app">
		{{msg}}
	</div>
</body>
<script>
	let vm = new Vue({
		el:"#app",
		data:{
			msg:"hello vue"
		},
		beforeCreate(){
			alert('实例创建前')
		},
		create(){
			alert('实例创建完成')
		},
		beforeMount(){
			alert('实例挂在前')
		},
		mounted(){
			alert('实例挂在完成')
		},
		updated(){
			alert('实例修改前')
		},
		beforeDestroy(){
			alert('实例删除')
		},
		destroyed(){
			alert('实例已经销毁')
		}
	})
</script>
</html>