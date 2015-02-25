TODO 01
========

* 지금부터 간단한 게임을 만듭니다.
* 아래 GameTetris() 함수를 구현해주세요.

```javascript
	function GameTetris() {
		
		//
		// TO DO : initGame 함수(객체)를 구현해주세요.
		//  
		//  - 해당 함수를 호출하면 지정된 ID 태그 안에 지정된 행과 열의 테이블을 생성합니다.
		//  예) gameTetris = new GameTetris();
		//		gameTetris.initGame("gameZone", // 게임을 위한 테이블이 추가될 html id
		//                          20,         // 테이블의 행 개수
		//                          12          // 테이블의 열 개수
		//                          );
		//
	
	}

```
	

	
> 초기 화면

![TODO01](https://raw.githubusercontent.com/lightsh/jsstudy/master/13/todo/images/todo_01.png)



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
				padding: 15px;
			}
			
			
		</style>
		<script type="text/javascript">
			
		
			function GameTetris() {
				
			}
			
			var gameTetris;
			window.onload = function() {
				gameTetris = new GameTetris();
				gameTetris.initGame("gameZone", 20, 12);
			}
				
		</script>
	</head>
<body>
<div>
	<div id="gameZone"/>
</div>
</body>
</html>

```
