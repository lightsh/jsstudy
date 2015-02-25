TODO 05
========

	
* 결과 화면처럼 총알이 녹색을 하나씩만 없애도록 합니다.

	
> 초기 화면

![TODO05](https://raw.githubusercontent.com/lightsh/jsstudy/master/12/todo/images/todo_05.png)


>  결과 화면 - 스페이스 키를 눌렀을 때

![TODO05](https://raw.githubusercontent.com/lightsh/jsstudy/master/12/todo/images/todo_05_result_01.gif)



## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<meta charset="UTF-8">
		<style type="text/css">
		
			table, th, td {
				border: 1px solid gray;
				border-collapse: collapse;
			}
			
			th, td {
				padding: 20px;
			}
			
			.player {
                background-color: rgb(51, 102, 204);
			}
					
			.bullet {
                background-color: rgb(221, 51, 85);
			}
			
			.enemy {
                background-color: rgb(43, 153, 91);
			}
			
		</style>
		<script type="text/javascript">
		
		</script>
	</head>
<body>
	<table> 
		<tr>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>			
			<td></td>
		</tr>
		<tr>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>			
			<td></td>
		</tr>
		<tr>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>			
			<td></td>
		</tr>
		<tr>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>			
			<td></td>
		</tr>
		<tr>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>			
			<td></td>
		</tr>
		<tr>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>			
			<td></td>
		</tr>
		<tr>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>			
			<td></td>
		</tr>
		<tr>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>			
			<td></td>
		</tr>
		<tr>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>			
			<td></td>
		</tr>
		<tr>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>			
			<td></td>
		</tr>
		<tr>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>
			<td></td>
			<td></td>	
			<td></td>
			<td></td>		
			<td></td>			
			<td></td>
		</tr>				
	</table>
</body>
</html>
```
