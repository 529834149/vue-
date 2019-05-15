<!doctype html>
<html lang="en">
<head>
	<meta charset="UTF-8" />
	<title>全选</title>
	<link rel="stylesheet" href="./node_modules/bootstrap/dist/css/bootstrap.min.css">
	<script src="../vue.js"></script>
</head>
<body>
	<div id="app" class="container">
		<div class="row">
			<h2 class="page-header">v-bind学习</h2>
			<table class="table table-bordered" border="" cellspacing="" cellpadding="">
				<tr>
					<th><input type="checkbox" velue="true" v-bind:checked="i" v-model="i" />全选</th>
					<th>书名</th>
					<th>价格</th>
					<th>数量</th>
				</tr>
				<tr v-for="book in books">
					<td><input type="checkbox" v-bind:checked="i"  /></td>
					<td>{{book.bookname}}</td>
					<td>{{book.price}}</td>
					<td>{{book.count}}</td>
				</tr>
			</table>
			
		</div>
	</div>
	
	
</body>
<script>
	let app  = new Vue({
		el:"#app",
		data:{
			s:"",
			i:false,
			books:[
				{bookname:"python",'price':10,count:1},
				{bookname:"python",'price':10,count:1},
				{bookname:"python",'price':10,count:1},
				{bookname:"python",'price':10,count:1},
				{bookname:"python",'price':10,count:1},
				{bookname:"python",'price':10,count:1},
			
			]
		}
	})
	
</script>
</html>