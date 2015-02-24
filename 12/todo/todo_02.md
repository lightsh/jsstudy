TODO 02
========

* 스페이스(Space)키를 누르면  초기화면 처럼 총알을 발사 시켜주세요.
	* 파란색(Player)이 위치한 셀을 기준으로 위쪽 방향으로 발사 시켜주세요.
	* 총알은 CSS 에서 클래스 bullet 을 사용해주세요

	
> 초기 화면

![TODO02](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/12/todo/images/todo_02.png)


>  결과 화면 - 스페이스 키를 눌렀을 때

![TODO02](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/12/todo/images/todo_02_result_01.png)


>  결과 화면 - 오른쪽 이동

![TODO02](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/12/todo/images/todo_02_result_02.png)


>  결과 화면 - 다시 스페이스 키를 눌렀을 때

![TODO02](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/12/todo/images/todo_02_result_03.png)


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
