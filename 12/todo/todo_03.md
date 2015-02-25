TODO 03
========

* 스페이스(Space)키를 누르면  초기화면 처럼 총알을 발사 시켜주세요.
	* 파란색(Player)이 위치한 셀을 기준으로 위쪽 방향으로 발사 시켜주세요.
	* 총알은 CSS 에서 클래스 bullet 을 사용해주세요
	
* TODO 02와 다르게 타이머를 사용해서 총알이 움직이는 것처럼 보이게 해주세요.
	* setInterval 함수를 사용하세요.

	
> 초기 화면

![TODO03](https://raw.githubusercontent.com/lightsh/jsstudy/master/12/todo/images/todo_03.png)


>  결과 화면 - 스페이스 키를 눌렀을 때

![TODO03](https://raw.githubusercontent.com/lightsh/jsstudy/master/12/todo/images/todo_03_result_02.gif)



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
