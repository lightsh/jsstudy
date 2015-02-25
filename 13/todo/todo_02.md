TODO 02
========

* 지금부터 간단한 게임을 만듭니다.
* 아래 GameTetris() 함수를 구현해주세요.

```javascript
	function GameTetris() {
		
		//
		// TO DO : initGame 함수를 구현해주세요.
		//  
		//  - 해당 함수를 호출하면 지정된 ID 태그 안에 지정된 행과 열의 테이블을 생성합니다.
		//  예) gameTetris = new GameTetris();
		//		gameTetris.initGame("gameZone", // 게임을 위한 테이블이 추가될 html id
		//                          20,         // 테이블의 행 개수
		//                          12          // 테이블의 열 개수
		//                          );
		//
	
	
		//
		// TO DO : startGame 함수를 구현해주세요.
		//  
		//  - 테이블 1행 1열에 2X2 파란색 블럭을 생성해 주세요.(css 에서 block 을 사용)
		//  - 2X2 파란색 블럭은 0.5 초 단위로 한 칸씩 밑으로 내려 갑니다.
		//  - 2X2 파란색 블럭이 움직이는 동안에 방향키(왼쪽, 오른쪽만)에 따라 움직여야 합니다. 
		//  - 2X2 파란색 블럭은 테이블의 마지막 또는 파란색 블럭을 만나면 멈추고 그 자리에 고정됩니다.
		
	}

```
	

	
> 초기 화면

![TODO02](https://raw.githubusercontent.com/lightsh/jsstudy/master/13/todo/images/todo_02.gif)



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
			
			.block {
                background-color: rgb(51, 102, 204);
			}
			
		</style>
		<script type="text/javascript">
			
		
			function GameTetris() {
				
			
			}
			
			var gameTetris;
			window.onload = function() {
				gameTetris = new GameTetris();
				gameTetris.initGame("gameZone", 20, 12);				
				document.getElementById("startGame").onclick = function() {
					gameTetris.startGame();
				}
			}
						
				
		</script>
	</head>
<body>
<div>
	<div id="gameZone"/>
</div>
<br>
<input type="button" id="startGame" value="start"/>
</body>
</html>

```
