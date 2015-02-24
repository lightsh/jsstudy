TODO 01
========

* 지금부터 간단한 게임을 만듭니다.
* 아래 초기 화면 처럼 11X11의 테이블을 구성해주세요.
	* 맨 아래쪽 행 중앙 셀의 배경색을 파란색(Player) 비슷꾸리한 것으로 해주세요.(CSS 에서 클래스 player 을 사용해주세요)
* 방향키를 눌러서 파란색(Player) 셀을 옮겨 주세요.
	* 왼쪽 키를 누르면 왼쪽으로 한 칸 이동해주세요.
	* 오른쪽 키를 누러면 오른쪽으로 한 칸 이동해주세요.
	* 윗쪽/아래쪽으로는 움직이지 않습니다.
	
* 코딩할 때 주의 사항.
	* 방향키는 window.onkeydown 을 사용해주세요.

	
> 초기 화면

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/12/todo/images/todo_01.png)


>  결과 화면 - 왼쪽 방향키를 눌렀을 때

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/12/todo/images/todo_01_result_01.png)


>  결과 화면 - 오른쪽 방향키를 눌렀을 때

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/12/todo/images/todo_01_result_02.png)



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
