1. 三张图片居左、居中、居右

```html
<!DOCTYPE html>
<html>
	<head>
		<style>
			.center{
			 	text-align: center;
			}
			.left{
				float: left;
			}
			.right{
				float:right;
			}
		</style>
	</head>
	<body>
		<div class="center">
			<img src="http://www.w3schools.com/images/w3html.gif" class="left">
			<img src="http://www.w3schools.com/images/w3css.gif">
			<img src="http://www.w3schools.com/images/w3javascript.gif" class="right">
		</div>
	</body>
</html>
```


2. 4行x3列的表格

```html
<!DOCTYPE html>
<html>
	<head>
		<style>
			table {
				 width:300px;
			}
			table,tr {
				border-bottom:1px solid black;
				border-collapse:collapse;
			}
			table,tr:last-child {
				border-bottom: none;
			}
		</style>
	</head>
	<body>
		<table>
			<tr>
  				<td>Jill</td>
  				<td>Smith</td>		
  				<td>50</td>
			</tr>
			<tr>
  				<td>Eve</td>
  				<td>Jackson</td>		
  				<td>94</td>
			</tr>
			<tr>
  				<td>John</td>
  				<td>Doe</td>		
  				<td>80</td>
			</tr>
			<tr>
  				<td>Monica</td>
  				<td>Jones</td>		
  				<td>20</td>
			</tr>
		</table>
	</body>
</html>
```


3. 图片被点击后，顺序顺时针移动

```html
<!DOCTYPE html>
<html>
	<head>
		<style>
			.center{
			 	text-align: center;
			}
			.left{
				float: left;
			}
			.right{
				float:right;
			}
		</style>
		<script>
			function rotate() {
				document.getElementsByClassName('left')[0].className='change-later';
    			document.getElementsByClassName('none')[0].className='left';
				document.getElementsByClassName('right')[0].className='none';
    			document.getElementsByClassName('change-later')[0].className='right';
			}
		</script>
	</head>
	<body>
		<div class="center">
			<img src="http://www.w3schools.com/images/w3html.gif" class="left" onclick="rotate()">
			<img src="http://www.w3schools.com/images/w3css.gif" class="none" onclick="rotate()">
			<img src="http://www.w3schools.com/images/w3javascript.gif" class="right" onclick="rotate()">
		</div>
	</body>
</html>
```
