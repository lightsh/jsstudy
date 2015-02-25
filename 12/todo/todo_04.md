TODO 04
========

* 테이블 상단 4개 행을 녹색(적군)으로 표시해주세요.
	* 녹색은 CSS 에서 클래스 enemy 을 사용해주세요
	
* 총알이 녹색을 지나면 녹색을 없애주세요.

	
> 초기 화면

![TODO04](https://raw.githubusercontent.com/lightsh/jsstudy/master/12/todo/images/todo_04.png)


>  결과 화면 - 스페이스 키를 눌렀을 때

![TODO04](https://raw.githubusercontent.com/lightsh/jsstudy/master/12/todo/images/todo_04_result_01.gif)



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
