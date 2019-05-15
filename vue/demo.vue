<!DOCTYPE html>
<html lang="zh">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<meta http-equiv="X-UA-Compatible" content="ie=edge">
	<link rel="stylesheet" href="./node_modules/bootstrap/dist/css/bootstrap.min.css">
	<title></title>
	<script src="../vue.js"></script>
	<!-- E:\xampp\htdocs\vue\vue\node_modules\_bootstrap@4.3.1@bootstrap\dist\css -->
</head>
<body>
	<!-- view 表达式大写-->
	<!-- <div id="app">
		<input type="text" v-model="msg">
		{{msg}} -->
	<!--  {{message.toUpperCase()}}
	  {{msg > 2 ? "yes" : "no"}} -->
	<!-- </div> -->
	<!-- <div id="app-2">
		<span v-bind:title="message"> 
			我喜欢你1
		</span>
	</div> -->
	<!-- <div id="app-3">
	  <p v-if="seen">现在你看到我了</p>
	</div> -->
	<!-- <div id="app-4">
	  <ol>
		<li v-for="todo in todos">
		  {{ todo.text }}
		</li>
	  </ol>
	</div> -->
	<!-- <div id="app-5">
		  <p>{{ message }}</p>
		  <button v-on:click="reverseMessage">逆转消息</button>
	</div> -->
	
	<!-- select双向绑定 -->
	<!-- <div id='app' class="container">
		<select name="" id="" v-model="msg">
			<option value="one">one</option>
			<option value="two">two</option>
			<option value="three">three</option>
			<option value="four">four</option>
			<option value="five">five</option>
			<option value="six">six</option>
		</select>
		<hr>
		<div class="bg-primary">{{msg}}</div>
	</div>
	 -->
	<div id="app" class="container">
		<div class="page-header">vue实例</div>
		<input type="text" v-model.trim="msg">
		{{msg.length}}
		<!-- <div class="row">
			<div class="col-md-6">
				<div class="jumbotron">
					<p>留言板</p>
					<div>{{msg}}</div>
				</div>
			</div>
			<div class="col-md-6">
				<textare cols="30" rows="10" class="form-control" v-model.lazy="msg"></textare>
			</div>
		</div>
		<div class="row">
			<input type="radio" v-model="msg" value="one">one
			<input type="radio" v-model="msg" value="two">two
			<input type="radio" v-model="msg" value="three">three
		</div>
		<div class="row">
			<input type="checkbox" v-model="arr" value="one">one
			<input type="checkbox" v-model="arr" value="two">two
			<input type="checkbox" v-model="arr" value="three">three
			<div class="bg-primary">{{arr}}</div>
		</div> -->
	</div>
</body>
<script>
	// var app2 = new Vue({
	//   el: '#app-2',
	//   data: {
	// 	message: '页面加载于 ' + new Date().toLocaleString(),
	// 	msg :10,
	//   }
	// })
	// var app3 = new Vue({
	// 	el:"#app-3",
	// 	data:{
	// 		seen: true
	// 	}
	// })
	// var app4 = new Vue({
	//   el: '#app-4',
	//   data: {
	// 	todos: [
	// 	  { text: '学习 JavaScript' },
	// 	  { text: '学习 Vue' },
	// 	  { text: '整个牛项目' }
	// 	]
	//   }
	// })
	var app = new Vue({
		 el:"#app",
		 data:{
			 msg: "",
			 num:10,
			 arr:[]
		 }
	})
</script>
</html>