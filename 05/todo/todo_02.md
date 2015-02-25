TODO 02
========

* 아래 sum() 함수를 구현해주세요.

```javascript
function sum() {
	var a01 = 1;
	var a02 = 2;
	var a03 = 3;
	var a04 = "4";  // 문자열 "4" 
	var a05 = 5;
	var a06 = 6;
	var a07 = "7";  // 문자열 "7"
	var a08 = 8;
	var a09 = 9;
	var a10 = 10;
	
	//
	// TO DO : 위에 선언한 변수들의 값을 모두 더한 결과를 리턴하는 코드를 작성해주세요.
	//
}

```

> 초기 화면

![TODO02](https://raw.githubusercontent.com/lightsh/jsstudy/master/05/todo/images/todo_02.png)


>  결과 화면

![TODO02](https://raw.githubusercontent.com/lightsh/jsstudy/master/05/todo/images/todo_02_result.png)

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
				var a04 = "4";  // 문자열 "4" 
				var a05 = 5;
				var a06 = 6;
				var a07 = "7";  // 문자열 "7"
				var a08 = 8;
				var a09 = 9;
				var a10 = 10;
				
			}
			
			function init() {
					document.getElementById("calculate").onclick = function() {
					var value = sum();
					document.getElementById("result").value = value;
					
				};
			}			
		</script>
	</head>
<body onload="init()">               
	<input type="button" id="calculate" value="calculate"/>        
	<input type="text" id="result"/> 
</body>
</html>

```
