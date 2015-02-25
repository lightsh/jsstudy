TODO 06
========

* 아래 sum() 함수를 구현해주세요.
* Math.max 함수 사용하지 마세요.

```javascript
function sum() {
	var a01 = 1;
	var a02 = 2;
	var a03 = 3;
	var a04 = 4;
	var a05 = 5;
	var a06 = 6;
	var a07 = 7;
	var a08 = 8;
	var a09 = 9;
	var a10 = 10;
	var list = [];
	
	//
	// TO DO : 아래 처럼 코드를 작성해주세요.
	// 1. 선언한 변수값을 차례대로 배열 list 에 담습니다.
	// 2. for 문을 사용하여 배열 list 에 담긴 값을 모두 합산합니다.
	// 3. 합산 결과를 리턴합니다.
}

```

> 초기 화면

![TODO06](https://raw.githubusercontent.com/lightsh/jsstudy/master/05/todo/images/todo_06.png)


>  결과 화면

![TODO06](https://raw.githubusercontent.com/lightsh/jsstudy/master/05/todo/images/todo_06_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
		</style>
		<script type="text/javascript">
			function sum() {
				var a01 = 1;
				var a02 = 2;
				var a03 = 3;
				var a04 = 4;
				var a05 = 5;
				var a06 = 6;
				var a07 = 7;
				var a08 = 8;
				var a09 = 9;
				var a10 = 10;
				var list = [];
			}
			
			function init() {
					document.getElementById("calculation").onclick = function() {
					var value = sum();
					document.getElementById("result").value = value;
					
				};
			}			
		</script>
	</head>
<body onload="init()">               
	<input type="button" id="calculation" value="calculation"/>        
	<input type="text" id="result"/> 
</body>
</html>

```
