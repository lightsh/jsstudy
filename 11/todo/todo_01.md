TODO 01
========

* 지금부터 간단한 게임을 만듭니다.
* 아래 초기 화면 처럼 도형으로 채워진 3X4의 테이블을 구성해주세요.
* 테이블의 컬럼 하단에 `down` 버튼을 만들어 주세요.
	* `down` 버튼을 클릭하면 해당 열의 도형을 아래 방향으로 회전 시켜주세요.
* 테이블의 행 오른쪽 끝에 `right->` 버튼을 만들어 주세요.
	* `right->` 버튼을 클릭하면 해당 행의 도형을 오른쪽 방향으로 회전 시켜주세요.
* `down`, `right->` 을 눌러 도형을 회전 시키다가 같은 도형이 2X2로 되면 하트 모양으로 변경해주세요.
* 모든 도형이 하트 모양으로 변경되면 `Good Job! Game Over!` 라는 메시지를 뿌려 줍니다.
* 도형의 모양은 css 를 사용하세요.

| 모양          | class         | 
| ------------- |:-------------:|
| 사각형        | rectangle     |
| 원            | circle        |
| 삼각형        | triangle      |
| 하트          | heart         |
	
* 코딩할 때 주의 사항.
	* innerHTML 사용하지 마세요.
	* 전역 변수(Global) 사용하지 마세요.
	* 버튼의 onclick 이벤트는 javascript 를 사용해서 바인딩해주세요.
	
> 초기 화면

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/11/todo/images/todo_01.png)


>  결과 화면 - down 버튼을 눌렀을 때

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/11/todo/images/todo_01_result_01.png)


>  결과 화면 - right 버튼을 눌렀을 때

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/11/todo/images/todo_01_result_02.png)


>  결과 화면 - 같의 모양의 2x2 로 될 경우(1)

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/11/todo/images/todo_01_result_03.png)


>  결과 화면 - 같의 모양의 2x2 로 될 경우(2)

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/11/todo/images/todo_01_result_04.png)


>  결과 화면 - GameOver

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/11/todo/images/todo_01_result_05.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<meta charset="UTF-8">
		<style type="text/css">
		
			td {
				text-align: center;
			}
			
			.rectangle {
				width: 100px;
				height: 100px;
                background-color: rgb(51, 102, 204);
                border: 1px solid rgb(44, 91, 104);      				
			}
			
			.circle {
				width: 100px;
				height: 100px;	
				background-color: rgb(51, 102, 204);
                border: 1px solid rgb(44, 91, 104);   
				-moz-border-radius: 50px;
				-webkit-border-radius: 50px;
				border-radius: 50px;			
			}
			
			.triangle {
				width: 0;
				height: 0;
				border-left: 50px solid transparent;
				border-right: 50px solid transparent;
				border-bottom: 100px solid rgb(51, 102, 204);
			}
				
			.heart {
				 position: relative;
				 width: 100px;
				 height: 100px;
			}
			
			.heart:before, .heart:after {
				 position: absolute;
				 content: "";
				 left: 50px;
				 top: 0;
				 width: 50px;
				 height: 80px;
				 background: rgb(221,51,85);
				 -moz-border-radius: 50px 50px 0 0;
				 border-radius: 50px 50px 0 0;
				 -webkit-transform: rotate(-45deg);
				 -moz-transform: rotate(-45deg);
				 -ms-transform: rotate(-45deg);
				 -o-transform: rotate(-45deg);
				 transform: rotate(-45deg);
				 -webkit-transform-origin: 0 100%;
				 -moz-transform-origin: 0 100%;
				 -ms-transform-origin: 0 100%;
				 -o-transform-origin: 0 100%;
				 transform-origin: 0 100%;
			}
			
			.heart:after {
				 left: 0;
				 -webkit-transform: rotate(45deg);
				 -moz-transform: rotate(45deg);
				 -ms-transform: rotate(45deg);
				 -o-transform: rotate(45deg);
				 transform: rotate(45deg);
				 -webkit-transform-origin: 100% 100%;
				 -moz-transform-origin: 100% 100%;
				 -ms-transform-origin: 100% 100%;
				 -o-transform-origin: 100% 100%;
				 transform-origin :100% 100%;
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
		</tr>
		<tr>
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
		</tr>
		<tr>
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
